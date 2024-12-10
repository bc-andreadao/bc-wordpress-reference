***

# Customer_Login_Request





* Full name: `\BigCommerce\Merchant\Models\Customer_Login_Request`
* This class implements:
[`\JsonSerializable`](../../../JsonSerializable.md)



## Properties


### store_hash



```php
private string $store_hash
```






***

### redirect_to



```php
private string $redirect_to
```






***

### channel_id



```php
private int $channel_id
```






***

## Methods


### __construct

Connect_Account_Request constructor.

```php
public __construct(string $store_hash, string $redirect_to = &#039;&#039;, int $channel_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$store_hash` | **string** |  |
| `$redirect_to` | **string** |  |
| `$channel_id` | **int** |  |





***

### jsonSerialize



```php
public jsonSerialize(): mixed
```












***


***
> Automatically generated on 2024-12-10
