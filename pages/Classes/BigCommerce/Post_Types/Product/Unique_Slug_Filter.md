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


***
> Automatically generated on 2025-01-07
