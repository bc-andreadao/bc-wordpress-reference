***

# Unique_Slug_Filter

Class Unique_Slug_Filter

Responsible for filtering the unique slug proposed
for a product, enforcing uniqueness per channel
but not globally

* Full name: `\BigCommerce\Post_Types\Product\Unique_Slug_Filter`




## Methods


### get_unique_slug



```php
public get_unique_slug(string $slug, int $post_id, string $post_status, string $post_type, int $post_parent, string $original_slug): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$slug` | **string** | The post slug, as deduplicated by WP. |
| `$post_id` | **int** | Post ID. |
| `$post_status` | **string** | The post status. |
| `$post_type` | **string** | Post type. |
| `$post_parent` | **int** | Post parent ID |
| `$original_slug` | **string** | The original post slug. |





***

### get_assigned_channel

Get the channel term assigned to the post

```php
private get_assigned_channel(int $post_id): \WP_Term
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** |  |





***

### is_unique_in_channel

Identify if the given slug is unique in the context of the given channel

```php
private is_unique_in_channel(string $slug, int $post_id, \WP_Term $channel): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$slug` | **string** |  |
| `$post_id` | **int** |  |
| `$channel` | **\WP_Term** |  |





***

### get_slug_blacklist



```php
private get_slug_blacklist(): mixed
```












***


***
> Automatically generated on 2024-12-10
