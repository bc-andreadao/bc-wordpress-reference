***

# Reset_Listing

Class Reset_Listing

Resets listing data to defaults, reconnecting its title
and description to the base product.

* Full name: `\BigCommerce\Post_Types\Product\Reset_Listing`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;reset-listing&#039;|


## Methods


### add_row_action

Adds a custom action link to the post row actions for products.

```php
public add_row_action(array $actions, \WP_Post $post): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$actions` | **array** | The current post row actions. |
| `$post` | **\WP_Post** | The post object. |


**Return Value:**

Modified post row actions.




***

### has_overrides

Checks if the product listing overrides base product fields.

```php
public has_overrides(\WP_Post $post): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post` | **\WP_Post** | The product post. |


**Return Value:**

True if overrides exist, false otherwise.




***

### get_reset_url

Generates the URL for resetting a product listing.

```php
public get_reset_url(\WP_Post $post): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post` | **\WP_Post** | The product post. |


**Return Value:**

The reset URL.




***

### handle_request

Handles the reset listing request.

```php
public handle_request(): void
```

Validates the request, resets the listing, and redirects the user.










***


***
> Automatically generated on 2025-01-14
