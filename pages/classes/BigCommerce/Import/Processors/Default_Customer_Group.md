***

# Default_Customer_Group





* Full name: `\BigCommerce\Import\Processors\Default_Customer_Group`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`DEFAULT_GROUP`|public| |&#039;bigcommerce_customers_default_group&#039;|


## Methods


### __construct



```php
public __construct(\BigCommerce\Api\v3\Api\PriceListsApi $price_list_api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$price_list_api` | **\BigCommerce\Api\v3\Api\PriceListsApi** |  |





***

### run



```php
public run(): mixed
```












***

### get_default_group

Retrieve group_ids from Price Collection Assignments and get first default customer group

```php
protected get_default_group(): false|mixed
```












***

### get_default_customer_groups



```php
protected get_default_customer_groups(): array|null
```












***


***
> Automatically generated on 2024-12-10
