***

# Amp_Cart_Menu_Item

Class Amp_Cart_Menu_Item

Enhances the cart menu item with AMP-specific functionality, such as adding classes
and dynamic cart item counts using AMP components.

* Full name: `\BigCommerce\Amp\Amp_Cart_Menu_Item`




## Methods


### add_classes_to_cart_page

Adds AMP-specific classes and cart item count functionality to the cart menu item.

```php
public add_classes_to_cart_page(object $menu_item, string $proxy_base): object
```

Adds a `menu-item-bigcommerce-cart` class to the cart menu item and replaces the
menu item's title with dynamic AMP-powered content that displays the current cart item count.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$menu_item` | **object** | The menu item object. |
| `$proxy_base` | **string** | The base URL or namespace used for proxying API requests. |


**Return Value:**

Filtered menu item with added AMP-specific functionality.




***


***
> Automatically generated on 2024-12-31
