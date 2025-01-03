***

# Item_Counter

Provides functionality to count the number of items in a BigCommerce cart.

This excludes child items, such as product variations or bundled items.

* Full name: `\BigCommerce\Cart\Item_Counter`




## Methods


### count_bigcommerce_cart

Count the total number of items in a BigCommerce cart.

```php
public static count_bigcommerce_cart(\BigCommerce\Api\v3\Model\Cart $cart): int
```

This method iterates through the items in the provided cart and calculates the total count.
It excludes child items (e.g., variations or bundled items) from the total count. If the quantity
of an item is available, it adds the quantity to the count; otherwise, it assumes a quantity of 1.

* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cart` | **\BigCommerce\Api\v3\Model\Cart** | The cart object to count items for. |


**Return Value:**

The total number of items in the cart.




***


***
> Automatically generated on 2025-01-03
