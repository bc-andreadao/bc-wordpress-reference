***

# Cart_Menu_Item

The Cart_Menu_Item class is responsible for modifying WordPress navigation menu items
to display cart-related information. It specifically adds a cart item count to the menu
item representing the cart page and ensures the proper display of this count based on
various conditions like checkout settings and the status of the mini-cart.

This class listens for the `wp_setup_nav_menu_item` filter to inject the necessary
HTML and CSS classes into the cart menu item and modifies the menu item title to
include a dynamic cart item count. It also provides methods to determine whether
the cart count should be shown and verifies if a menu item corresponds to the cart page.

The Cart_Menu_Item class interacts with WordPress options and applies filters to
conditionally enable or disable cart item count display. It also provides hooks
for customizing cart-related functionality, making it adaptable to different configurations.

* Full name: `\BigCommerce\Cart\Cart_Menu_Item`




## Methods


### add_classes_to_cart_page

Adds classes to the cart page menu item and updates the title with the item count.

```php
public add_classes_to_cart_page(object $menu_item): object
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$menu_item` | **object** | The menu item object to modify. |


**Return Value:**

The modified menu item object.




***


***
> Automatically generated on 2025-01-13
