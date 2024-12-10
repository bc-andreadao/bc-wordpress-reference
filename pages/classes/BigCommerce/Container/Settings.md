***

# Settings

Provides various screens and settings for BigCommerce.

This class is responsible for registering settings screens, handling API credentials,
and managing various onboarding steps in the BigCommerce plugin.

* Full name: `\BigCommerce\Container\Settings`
* Parent class: [`Provider`](./Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`SETTINGS_SCREEN`|public|string|&#039;settings.screen.settings&#039;|
|`WELCOME_SCREEN`|public|string|&#039;settings.screen.welcome&#039;|
|`CREATE_SCREEN`|public|string|&#039;settings.screen.create&#039;|
|`STORE_TYPE_SCREEN`|public|string|&#039;settings.screen.store_type&#039;|
|`CHANNEL_SCREEN`|public|string|&#039;settings.screen.channel&#039;|
|`PENDING_SCREEN`|public|string|&#039;settings.screen.pending&#039;|
|`CREDENTIALS_SCREEN`|public|string|&#039;settings.screen.credentials&#039;|
|`MENU_SETUP_SCREEN`|public|string|&#039;settings.screen.nav_menu&#039;|
|`COMPLETE_SCREEN`|public|string|&#039;settings.screen.onboarding_complete&#039;|
|`RESOURCES_SCREEN`|public|string|&#039;settings.screen.resources&#039;|
|`API_SECTION`|public|string|&#039;settings.section.api&#039;|
|`CONNECT_ACCOUNT_SECTION`|public|string|&#039;settings.section.connect_account&#039;|
|`CART_SECTION`|public|string|&#039;settings.section.cart&#039;|
|`GIFT_CERTIFICATE_SECTION`|public|string|&#039;settings.section.gift_certificates&#039;|
|`CURRENCY_SECTION`|public|string|&#039;settings.section.currency&#039;|
|`IMPORT_SECTION`|public|string|&#039;settings.section.import&#039;|
|`ACCOUNTS_SECTION`|public|string|&#039;settings.section.accounts&#039;|
|`ANALYTICS_SECTION`|public|string|&#039;settings.section.analytics&#039;|
|`REVIEWS_SECTION`|public|string|&#039;settings.section.reviews&#039;|
|`NEW_ACCOUNT_SECTION`|public|string|&#039;settings.section.new_account&#039;|
|`SELECT_CHANNEL_SECTION`|public|string|&#039;settings.section.select_channel&#039;|
|`IMPORT_SETTINGS_SECTION`|public|string|&#039;settings.section.import_settings&#039;|
|`CHANNEL_SECTION`|public|string|&#039;settings.section.channel&#039;|
|`DIAGNOSTICS_SECTION`|public|string|&#039;settings.section.diagnostics&#039;|
|`MENU_OPTIONS_SECTION`|public|string|&#039;settings.section.nav_menu_options&#039;|
|`NEXT_STEPS_SECTION`|public|string|&#039;settings.section.next_steps&#039;|
|`API_STATUS`|public|string|&#039;settings.api_status&#039;|
|`IMPORT_NOW`|public|string|&#039;settings.import_now&#039;|
|`IMPORT_STATUS`|public|string|&#039;settings.import_status&#039;|
|`IMPORT_LIVE_STATUS`|public|string|&#039;settings.import_status_live&#039;|
|`START_OVER`|public|string|&#039;settings.start_over&#039;|
|`ONBOARDING_PROGRESS`|public|string|&#039;settings.onboarding.progress_bar&#039;|
|`SITE_URL_SYNC`|public|string|&#039;settings.site_url_sync&#039;|
|`ABORT_IMPORT`|public|string|&#039;settings.abort_product_import&#039;|
|`FLUSH_CACHE`|public|string|&#039;settings.flush_cache&#039;|
|`HEADLESS`|public|string|&#039;settings.headless_processing&#039;|
|`CONFIG_STATUS`|public|string|&#039;settings.configuration_status&#039;|
|`CONFIG_DISPLAY_MENUS`|public|string|&#039;settings.configuration_display_menus&#039;|
|`STATUS_NEW`|public|string|0|
|`STATUS_ACCOUNT_PENDING`|public|string|10|
|`STATUS_API_CONNECTED`|public|string|20|
|`STATUS_CHANNEL_CONNECTED`|public|string|40|
|`STATUS_STORE_TYPE_SELECTED`|public|string|50|
|`STATUS_MENUS_CREATED`|public|string|70|
|`STATUS_COMPLETE`|public|string|1000|


## Methods


### register

Registers settings and screens in the container.

```php
public register(\Pimple\Container $container): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | Dependency injection container. |





***

### settings_screen



```php
private settings_screen(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### api_credentials



```php
private api_credentials(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### api_status_indicator



```php
private api_status_indicator(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### cart



```php
private cart(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### gift_certificates



```php
private gift_certificates(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### import



```php
private import(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### currency



```php
private currency(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### next_steps



```php
private next_steps(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### accounts



```php
private accounts(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### analytics



```php
private analytics(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### reviews



```php
private reviews(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### onboarding



```php
private onboarding(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### onboarding_progress_bar



```php
private onboarding_progress_bar(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### set_menus_default_visibility

Handles menus visibility for the settings screen and nav menu page

```php
private set_menus_default_visibility(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### diagnostics



```php
private diagnostics(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### resources



```php
private resources(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***


***
> Automatically generated on 2024-12-10
