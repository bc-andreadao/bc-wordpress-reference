***

# Migrate_Blocks

Handles the migration of shortcodes to Gutenberg blocks in the editor. When a post is loaded in the
Gutenberg editor, this class manages the transition from legacy shortcodes to dynamic blocks
specific to the BigCommerce platform.

It provides methods to determine which editor (Gutenberg or Classic) is being used and
applies the necessary filters to migrate content.

* Full name: `\BigCommerce\Editor\Gutenberg\Migrate_Blocks`




## Methods


### check_if_gutenberg_editor

Checks if the Gutenberg editor will be used to edit the post, and sets up appropriate hooks
for filtering the post content if Gutenberg is the active editor.

```php
public check_if_gutenberg_editor(bool $passthrough, \WP_Post $post): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$passthrough` | **bool** | Indicates whether to bypass the migration (used by other filters). |
| `$post` | **\WP_Post** | The post object being edited. |


**Return Value:**

The filtered passthrough value, which determines whether to proceed with the content migration.




**See Also:**

* \BigCommerce\Editor\Gutenberg\gutenberg_init() - 

***

### check_if_classic_editor

Checks if the Classic editor will be used to edit the post, and sets up appropriate hooks
for filtering the post content if the Classic editor is active.

```php
public check_if_classic_editor(bool $passthrough, \WP_Post $post): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$passthrough` | **bool** | Indicates whether to bypass the migration (used by other filters). |
| `$post` | **\WP_Post** | The post object being edited. |


**Return Value:**

The filtered passthrough value, which determines whether to proceed with the content migration.




**See Also:**

* \BigCommerce\Editor\Gutenberg\gutenberg_init() - 

***

### set_gutenberg_editor_hooks



```php
private set_gutenberg_editor_hooks(\WP_Post $post): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post` | **\WP_Post** |  |





***

### set_classic_editor_hooks



```php
private set_classic_editor_hooks(mixed $post): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post` | **mixed** |  |





***

### filter_post_rest_response

Filters the REST API response for the post, ensuring that blocks are properly migrated
when the post content is fetched via the REST API.

```php
public filter_post_rest_response(\WP_REST_Response $response, \WP_Post $post, \WP_REST_Request $request): \WP_REST_Response
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$response` | **\WP_REST_Response** | The response object containing the post data. |
| `$post` | **\WP_Post** | The post object being fetched. |
| `$request` | **\WP_REST_Request** | The REST request object. |


**Return Value:**

The modified response object with migrated content.




***

### ensure_blocks



```php
private ensure_blocks(mixed $content): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$content` | **mixed** |  |





***

### product_shortcode_to_block



```php
private product_shortcode_to_block(mixed $match): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$match` | **mixed** |  |





***

### replace_blocks_with_shortcodes

Transform all bigcommerce blocks into their shortcode equivalents

```php
private replace_blocks_with_shortcodes(string $content): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$content` | **string** |  |





***


***
> Automatically generated on 2024-12-10