***

# Nav_Menu

Class Nav_Menu

Responsible for setting and filtering navigation menu items related to account pages.

* Full name: `\BigCommerce\Accounts\Nav_Menu`




## Methods


### filter_account_menu_items

Filters the account menu items based on the page ID.

```php
public filter_account_menu_items(object $menu_item): object
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$menu_item` | **object** | The menu item to filter. |


**Return Value:**

The filtered menu item.




***

### setup_login_menu_item

Sets up the login/logout menu item.

```php
public setup_login_menu_item(\WP_Post $menu_item): \WP_Post
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$menu_item` | **\WP_Post** | The menu item to modify. |


**Return Value:**

The modified menu item.




***

### setup_registration_menu_item

Adds the registration/signup menu item.

```php
public setup_registration_menu_item(\WP_Post $menu_item): \WP_Post
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$menu_item` | **\WP_Post** | The menu item to modify. |


**Return Value:**

The modified menu item.




***

### setup_account_page_menu_item

Sets up the account-related menu item.

```php
public setup_account_page_menu_item(\WP_Post $menu_item): \WP_Post
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$menu_item` | **\WP_Post** | The menu item to modify. |


**Return Value:**

The modified menu item.




***


***
> Automatically generated on 2025-01-07
