***

# Taxonomies

This class is responsible for managing and registering taxonomies for BigCommerce integration. It defines constants for various taxonomies and handles their configuration and filtering via WordPress hooks.



* Full name: `\BigCommerce\Container\Taxonomies`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`PRODUCT_CATEGORY`|public|string|&#039;taxonomy.product_category&#039;|
|`PRODUCT_CATEGORY_CONFIG`|public|string|&#039;taxonomy.product_category.config&#039;|
|`PRODUCT_CATEGORY_GROUP_FILTERED_TERMS`|public|string|&#039;taxonomy.product_category.group_filtered_terms&#039;|
|`PRODUCT_CATEGORY_QUERY_FILTER`|public|string|&#039;taxonomy.product_category.query_filter&#039;|
|`BRAND`|public|string|&#039;taxonomy.brand&#039;|
|`BRAND_CONFIG`|public|string|&#039;taxonomy.brand.config&#039;|
|`AVAILABILITY`|public|string|&#039;taxonomy.availability&#039;|
|`AVAILABILITY_CONFIG`|public|string|&#039;taxonomy.availability.config&#039;|
|`CONDITION`|public|string|&#039;taxonomy.condition&#039;|
|`CONDITION_CONFIG`|public|string|&#039;taxonomy.condition.config&#039;|
|`PRODUCT_TYPE`|public|string|&#039;taxonomy.product_type&#039;|
|`PRODUCT_TYPE_CONFIG`|public|string|&#039;taxonomy.product_type.config&#039;|
|`FLAG`|public|string|&#039;taxonomy.flag&#039;|
|`FLAG_CONFIG`|public|string|&#039;taxonomy.flag.config&#039;|
|`CHANNEL`|public|string|&#039;taxonomy.channel&#039;|
|`CHANNEL_CONFIG`|public|string|&#039;taxonomy.channel.config&#039;|
|`CHANNEL_SYNC`|public|string|&#039;taxonomy.channel.sync&#039;|
|`CHANNEL_CONNECTOR`|public|string|&#039;taxonomy.channel.connector&#039;|
|`CHANNEL_ADMIN_FILTER`|public|string|&#039;taxonomy.channel.admin_products_filter&#039;|
|`CHANNEL_QUERY_FILTER`|public|string|&#039;taxonomy.channel.query_filter&#039;|
|`CHANNEL_CURRENCY_FILTER`|public|string|&#039;taxonomy.channel.currency_filter&#039;|
|`CHANNEL_BC_STATUS`|public|string|&#039;taxonomy.channel.bc_status&#039;|
|`ROUTES`|public|string|&#039;taxonomy.channel.routes&#039;|


## Methods


### register

Registers all taxonomies and related actions and filters.

```php
public register(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The container object. |





***


***
> Automatically generated on 2024-12-13
