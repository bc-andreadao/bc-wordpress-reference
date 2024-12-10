***

# Accounts

Class Accounts

Handles the registration and initialization of various account-related services
such as login, registration, countries, wishlists, profile settings, and customer groups.

* Full name: `\BigCommerce\Container\Accounts`
* Parent class: [`Provider`](./Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`LOGIN`|public|string|&#039;accounts.login&#039;|
|`REGISTER`|public|string|&#039;accounts.register&#039;|
|`COUNTRIES`|public|string|&#039;accounts.countries&#039;|
|`COUNTRIES_PATH`|public|string|&#039;accounts.countries.path&#039;|
|`DELETE_ADDRESS`|public|string|&#039;accounts.delete_address&#039;|
|`NAV_MENU`|public|string|&#039;accounts.nav_menu&#039;|
|`SUB_NAV`|public|string|&#039;accounts.sub_nav&#039;|
|`USER_PROFILE`|public|string|&#039;accounts.user_profile&#039;|
|`GROUP_PROXY`|public|string|&#039;accounts.groups.proxy&#039;|
|`PASSWORD_RESET`|public|string|&#039;accounts.password_reset&#039;|
|`CHANNEL_SETTINGS`|public|string|&#039;accounts.channel_settings&#039;|
|`PUBLIC_WISHLIST`|public|string|&#039;accounts.wishlist.public&#039;|
|`WISHLIST_ROUTER`|public|string|&#039;accounts.wishlist.router&#039;|
|`WISHLIST_CREATE`|public|string|&#039;accounts.wishlist.create&#039;|
|`WISHLIST_EDIT`|public|string|&#039;accounts.wishlist.edit&#039;|
|`WISHLIST_DELETE`|public|string|&#039;accounts.wishlist.delete&#039;|
|`WISHLIST_ADD`|public|string|&#039;accounts.wishlist.add_item&#039;|
|`WISHLIST_REMOVE`|public|string|&#039;accounts.wishlist.remove_item&#039;|
|`WISHLIST_ADD_ITEM_VIEW`|public|string|&#039;accounts.wishlist.add_item_view&#039;|


## Methods


### register

Registers various services into the container

```php
public register(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container |





***

### login

Registers and handles login-related actions.

```php
private login(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container |





***

### countries

Registers and handles country-related services and requests.

```php
private countries(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container |





***

### profile

Registers profile-related services and actions.

```php
private profile(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container |





***

### addresses

Registers and handles address-related services and actions.

```php
private addresses(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container |





***

### customer_groups

Registers customer group-related services and actions.

```php
private customer_groups(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container |





***

### wishlists

Registers and handles wishlist-related services and actions.

```php
private wishlists(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The dependency injection container |





***

### passwords

Handle passwords container and hooks

```php
private passwords(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### channel_settings

Handle channel settings container and hooks

```php
private channel_settings(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***


***
> Automatically generated on 2024-12-10
