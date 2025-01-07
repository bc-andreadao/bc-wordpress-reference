***

# Webhooks

Provider for handling BigCommerce webhooks.

This class sets up webhook-related constants, services, and handlers
to process webhook requests, manage their lifecycle, and integrate
with BigCommerce APIs.

* Full name: `\BigCommerce\Container\Webhooks`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`WEBHOOKS`|public|string|&#039;webhooks.webhooks&#039;|
|`WEBHOOKS_STATUS`|public|string|&#039;webhooks.webhooks_status&#039;|
|`WEBHOOKS_LISTENER`|public|string|&#039;webhooks.listener_webhook&#039;|
|`CHANNELS_HANDLE_WEBHOOK`|public|string|&#039;webhooks.channels_handle_webhook&#039;|
|`PRODUCT_UPDATE_WEBHOOK`|public|string|&#039;webhooks.product_update_webhook&#039;|
|`PRODUCT_DELETE_WEBHOOK`|public|string|&#039;webhooks.product_delete_webhook&#039;|
|`PRODUCT_CREATE_WEBHOOK`|public|string|&#039;webhooks.product_create_webhook&#039;|
|`PRODUCT_INVENTORY_UPDATE_WEBHOOK`|public|string|&#039;webhooks.inventory_update_webhook&#039;|
|`CUSTOMER_CREATE_WEBHOOK`|public|string|&#039;webhooks.customer_create_webhook&#039;|
|`CUSTOMER_UPDATE_WEBHOOK`|public|string|&#039;webhooks.customer_update_webhook&#039;|
|`CUSTOMER_DELETE_WEBHOOK`|public|string|&#039;webhooks.customer_delete_webhook&#039;|
|`PRODUCT_UPDATER`|public|string|&#039;webhooks.cron.product_updater&#039;|
|`PRODUCT_CREATOR`|public|string|&#039;webhooks.cron.product_creator&#039;|
|`CHANNEL_PRODUCT_ASSIGNED`|public|string|&#039;webhooks.product.channels_assign&#039;|
|`CHANNEL_PRODUCT_UNASSIGNED`|public|string|&#039;webhooks.product.channels_unassign&#039;|
|`CHANNEL_UPDATER`|public|string|&#039;webhooks.product.channels_updater&#039;|
|`CHANNEL_CURRENCY_UPDATED`|public|string|&#039;webhooks.channels.currency_updated&#039;|
|`CUSTOMER_CREATOR`|public|string|&#039;webhooks.cron.customer_creator&#039;|
|`CUSTOMER_UPDATER`|public|string|&#039;webhooks.cron.customer_updater&#039;|
|`CUSTOMER_DELETER`|public|string|&#039;webhooks.cron.customer_deleter&#039;|
|`CUSTOMER_CHANNEL_ACCESS_UPDATER`|public|string|&#039;webhooks.cron.customer_channel_access_updater&#039;|
|`CUSTOMER_CHANNEL_ACCESS`|public|string|&#039;webhooks.cron.customer_channel_access&#039;|
|`CHECKOUT_COMPLETE_WEBHOOK`|public|string|&#039;webhooks.checkout_complete&#039;|
|`WEBHOOKS_VERSIONING`|public|string|&#039;webhooks.version&#039;|
|`WEBHOOKS_CRON_TASKS`|public|string|&#039;webhooks.cron_tasks&#039;|


## Methods


### register

Registers services related to webhooks in the container.

```php
public register(\Pimple\Container $container): void
```

Sets up webhook declarations, their statuses, and actions
for processing and managing webhook events.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The Pimple container instance. |





***


***
> Automatically generated on 2025-01-07
