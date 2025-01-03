***

# Dynamic_Menu_Items





* Full name: `\BigCommerce\Nav_Menu\Dynamic_Menu_Items`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`TYPE`|public| |&#039;bigcommerce_dynamic&#039;|


## Methods


### setup_menu_item



```php
public setup_menu_item(object $item): object
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$item` | **object** |  |





***

### insert_dynamic_menu_items

Add the child terms under the top-level dynamic menu items

```php
public insert_dynamic_menu_items(array $items, object $menu, array $args): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$items` | **array** | An array of menu item post objects. |
| `$menu` | **object** | The menu object. |
| `$args` | **array** | An array of arguments used to retrieve menu item objects. |





***


***
> Automatically generated on 2025-01-03
