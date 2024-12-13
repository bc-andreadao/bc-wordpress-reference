***

# Settings

Provides various screens and settings for BigCommerce.

This class is responsible for registering settings screens, handling API credentials,
and managing various onboarding steps in the BigCommerce plugin.

* Full name: `\BigCommerce\Container\Settings`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


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


***
> Automatically generated on 2024-12-13
