***

# Product_Remover

Handles the removal of products from WordPress by matching them with their
corresponding BigCommerce product IDs and channel terms.

This class provides methods for deleting products either by WordPress post ID
or by matching a BigCommerce product ID with its associated WordPress post.
It also ensures that the correct product is targeted based on the channel term
associated with the product.

* Full name: `\BigCommerce\Import\Importers\Products\Product_Remover`




## Methods


### remove_by_post_id

Removes a product by its WordPress post ID.

```php
public remove_by_post_id(int $post_id): mixed
```

This method will delete the product post from WordPress if the post ID is not empty.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** | The WordPress post ID of the product to be removed. |





***

### remove_by_product_id

Removes a product by its BigCommerce product ID and channel term.

```php
public remove_by_product_id(int $product_id, \WP_Term $channel): mixed
```

This method will first match the WordPress post ID for the given BigCommerce product ID and channel,
then proceed to remove the corresponding WordPress post.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **int** | The BigCommerce product ID. |
| `$channel` | **\WP_Term** | The WordPress term representing the channel to which the product belongs. |





***


***
> Automatically generated on 2025-01-07
