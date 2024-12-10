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

### get_menu_item_children

Get the top-level terms from the taxonomy as menu items

```php
private get_menu_item_children(object $item): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$item` | **object** |  |





***

### get_terms_items



```php
private get_terms_items(mixed $taxonomy, int $parent): array|int[]|string|string[]|\WP_Error|\WP_Term[]
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$taxonomy` | **mixed** |  |
| `$parent` | **int** |  |





***


***
> Automatically generated on 2024-12-10
