***

# Create_Account_Request





* Full name: `\BigCommerce\Merchant\Models\Create_Account_Request`
* This class implements:
[`\JsonSerializable`](../../../JsonSerializable.md)



## Properties


### secret_key



```php
private string $secret_key
```






***

### store_name



```php
private string $store_name
```






***

### store_url



```php
private string $store_url
```






***

### contact



```php
private \BigCommerce\Merchant\Models\Account_Contact $contact
```






***

## Methods


### __construct



```php
public __construct(mixed $secret_key, mixed $store_name, mixed $store_url, \BigCommerce\Merchant\Models\Account_Contact $contact): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$secret_key` | **mixed** |  |
| `$store_name` | **mixed** |  |
| `$store_url` | **mixed** |  |
| `$contact` | **\BigCommerce\Merchant\Models\Account_Contact** |  |





***

### jsonSerialize



```php
public jsonSerialize(): mixed
```












***


***
> Automatically generated on 2024-12-10
