***

# Unsupported_Products





* Full name: `\BigCommerce\Post_Types\Product\Unsupported_Products`




## Methods


### disallow_publication

Users should not be permitted to publish unsupported posts.

```php
public disallow_publication(array $caps, string $cap, int $user_id, array $args): array
```

Unfortunately, WP does not provide granular caps for publishing
posts, so we are left with a blanket cap for publishing all
posts. We just apply this filter on the product single admin,
but can do nothing about quick edit in the products list table.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$caps` | **array** | Returns the user&#039;s actual capabilities. |
| `$cap` | **string** | Capability name. |
| `$user_id` | **int** | The user ID. |
| `$args` | **array** | Adds the context to the cap. Typically the object ID. |





***

### show_unsupported_status



```php
public show_unsupported_status(array $post_states, \WP_Post $post): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_states` | **array** |  |
| `$post` | **\WP_Post** |  |





***

### prevent_publication



```php
public prevent_publication(array $data, array $postarr): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **array** | An array of sanitized attachment post data. |
| `$postarr` | **array** | An array of unsanitized attachment post data. |





***


***
> Automatically generated on 2025-01-13
