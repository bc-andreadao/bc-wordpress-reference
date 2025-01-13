***

# Default_Customer_Group

Handles operations related to the default customer group for BigCommerce integrations.



* Full name: `\BigCommerce\Import\Processors\Default_Customer_Group`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`DEFAULT_GROUP`|public|string|&#039;bigcommerce_customers_default_group&#039;|


## Methods


### __construct

Constructor to initialize the Price Lists API.

```php
public __construct(\BigCommerce\Api\v3\Api\PriceListsApi $price_list_api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$price_list_api` | **\BigCommerce\Api\v3\Api\PriceListsApi** | API instance for Price Lists. |





***

### run

Main function to execute the default group processing.

```php
public run(): void
```












***

### get_default_group

Retrieve group IDs from Price Collection Assignments and fetch the first default customer group.

```php
protected get_default_group(): false|mixed
```









**Return Value:**

The ID of the default customer group or false if none found.




***

### get_default_customer_groups

Retrieve all default customer groups from BigCommerce.

```php
protected get_default_customer_groups(): array|null
```









**Return Value:**

An array of default customer group IDs or null if none found.




***


***
> Automatically generated on 2025-01-13
