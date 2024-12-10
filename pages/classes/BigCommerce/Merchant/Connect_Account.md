***

# Connect_Account





* Full name: `\BigCommerce\Merchant\Connect_Account`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`CONNECT_ACTION`|public| |&#039;bigcommerce_connect_account&#039;|

## Properties


### onboarding



```php
private \BigCommerce\Merchant\Onboarding_Api $onboarding
```






***

## Methods


### __construct



```php
public __construct(\BigCommerce\Merchant\Onboarding_Api $onboarding_api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$onboarding_api` | **\BigCommerce\Merchant\Onboarding_Api** |  |





***

### connect_account_url

Point the Connect Account button to the admin action URL we'll handle

```php
public connect_account_url(string $url): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$url` | **string** |  |





***

### connect_account



```php
public connect_account(): void
```












***

### generate_guid

Create a random GUID to use as a store identifier when
connecting to an existing store where we don't know its
store ID.

```php
private generate_guid(): string
```












***


***
> Automatically generated on 2024-12-10
