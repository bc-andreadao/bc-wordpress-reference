***

# Customer_Deleter





* Full name: `\BigCommerce\Webhooks\Customer\Customer_Deleter`
* Parent class: [`\BigCommerce\Webhooks\Customer\Customer_Saver`](./classes/BigCommerce/Webhooks/Customer/Customer_Saver.md)




## Methods


### handle_request

Delete single customer by id

```php
public handle_request(int $customer_id, array $channel_ids = []): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$customer_id` | **int** |  |
| `$channel_ids` | **array** |  |





***


## Inherited methods


### __construct



```php
public __construct(\BigCommerce\Api\v3\Api\CustomersApi $customers_api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$customers_api` | **\BigCommerce\Api\v3\Api\CustomersApi** |  |





***

### get_v3_customer_by_id

Get customer details via v3 API. v3 will return channels_ids that will be used later in channel aware logic

```php
protected get_v3_customer_by_id(int $customer_id): false|mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$customer_id` | **int** |  |





***

### handle_request

Handle webhook requests

```php
public handle_request(int $customer_id, array $channel_ids = []): bool
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$customer_id` | **int** |  |
| `$channel_ids` | **array** |  |





***

### get_by_bc_id

Get customer by BC id

```php
public get_by_bc_id(mixed $id): false|mixed|null
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$id` | **mixed** |  |





***

### get_customer_match



```php
public get_customer_match(int $customer_id): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$customer_id` | **int** |  |





***

### delete_customer



```php
protected delete_customer(int $customer_id): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$customer_id` | **int** |  |





***

### maybe_remove_customer_msf



```php
protected maybe_remove_customer_msf(\BigCommerce\Api\v3\Model\Customer $customer): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$customer` | **\BigCommerce\Api\v3\Model\Customer** |  |





***

### save_customer_channel_data



```php
protected save_customer_channel_data(\WP_User $user, \BigCommerce\Api\v3\Model\Customer $customer): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$user` | **\WP_User** |  |
| `$customer` | **\BigCommerce\Api\v3\Model\Customer** |  |





***


***
> Automatically generated on 2024-12-13
