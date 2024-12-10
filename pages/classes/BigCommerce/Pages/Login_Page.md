***

# Login_Page





* Full name: `\BigCommerce\Pages\Login_Page`
* Parent class: [`\BigCommerce\Pages\Required_Page`](./Required_Page.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public|string|&#039;bigcommerce_login_page_id&#039;|
|`SLUG`|public| |&#039;login&#039;|


## Methods


### get_title



```php
protected get_title(): string
```









**Return Value:**

The title of the post




***

### get_slug



```php
public get_slug(): string
```









**Return Value:**

The slug of the post




***

### get_content



```php
public get_content(): string
```









**Return Value:**

The content of the post




***

### get_post_state_label



```php
public get_post_state_label(): string
```









**Return Value:**

The label to show on this post in list tables




***


## Inherited methods


### __construct



```php
public __construct(): mixed
```












***

### get_option_name



```php
public get_option_name(): mixed
```












***

### get_post_type



```php
protected get_post_type(): string
```









**Return Value:**

The post type of the post that will be created




***

### get_title



```php
protected get_title(): string
```




* This method is **abstract**.




**Return Value:**

The title of the post




***

### get_slug



```php
protected get_slug(): string
```




* This method is **abstract**.




**Return Value:**

The slug of the post




***

### get_content



```php
public get_content(): string
```









**Return Value:**

The content of the post




***

### filter_content

Add page shortcode to the content if missing

```php
public filter_content(int $post_id, string $content): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** | Post id |
| `$content` | **string** | Post content |


**Return Value:**

The content of the post




***

### get_post_state_label



```php
public get_post_state_label(): string
```









**Return Value:**

The label to show on this post in list tables




***

### ensure_page_exists

Ensure that there is a page designated as this page
at all times. Creates one if necessary.

```php
public ensure_page_exists(): void
```












***

### clear_option_on_delete



```php
public clear_option_on_delete(mixed $post_id): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **mixed** |  |





***

### match_existing_post

Find an existing post that can be designated as the
required page.

```php
protected match_existing_post(): int
```









**Return Value:**

The ID of the matching post. 0 if none found.




***

### get_post_candidates

Find all the posts that meet the criteria (e.g., post type,
content) to become this required page.

```php
public get_post_candidates(bool $include_uninstalled = false): int[]
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$include_uninstalled` | **bool** | Whether the list of candidates should include<br />pages that have been uninstalled and set to draft |


**Return Value:**

Post IDs of potential posts




***

### create_post

Create the post for this config

```php
protected create_post(): int
```









**Return Value:**

the ID of the created post




***

### get_post_args



```php
protected get_post_args(): array
```









**Return Value:**

The args for creating the post




***

### add_post_state



```php
public add_post_state(array $post_states, \WP_Post $post): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_states` | **array** |  |
| `$post` | **\WP_Post** |  |





***


***
> Automatically generated on 2024-12-10
