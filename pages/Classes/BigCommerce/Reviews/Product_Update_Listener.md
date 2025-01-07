***

# Product_Update_Listener

Class Product_Update_Listener

Listens for updates to product meta to determine if the review
cache should be flushed

* Full name: `\BigCommerce\Reviews\Product_Update_Listener`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`TRIGGER_UPDATE`|public| |&#039;bigcommerce/reviews/update&#039;|


## Methods


### meta_updated

Check if updates to product meta include changes to review count or rating sum

```php
public meta_updated(int $meta_id, int $post_id, string $meta_key, mixed $meta_value): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$meta_id` | **int** | ID of updated metadata entry. |
| `$post_id` | **int** | Post ID. |
| `$meta_key` | **string** | Meta key. |
| `$meta_value` | **mixed** | Meta value. |





***


***
> Automatically generated on 2025-01-07
