***

# Currency

Handles currency operations, including fetching and setting currency codes and managing channel-aware currencies.



* Full name: `\BigCommerce\Currency\Currency`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`CURRENCY_CODE_COOKIE`|public| |&#039;wp-bigcommerce-currency-code&#039;|


## Methods


### get_currency_code

Retrieves the current currency code.

```php
public get_currency_code(): string
```

Determines the currency code based on user preferences, cookies, or channel-specific defaults.







**Return Value:**

The current currency code.




***

### set_currency_code

Sets the currency code for the current user and stores it in a cookie.

```php
public set_currency_code(string $currency_code): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$currency_code` | **string** | The currency code to set. |


**Return Value:**

True if the currency code was successfully set; otherwise, false.




***

### set_currency_code_cookie

Sets a cookie to store the currency code.

```php
public set_currency_code_cookie(string $currency_code): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$currency_code` | **string** | The currency code to store in the cookie. |





***

### get_channel_aware_currencies

Retrieves channel-aware currencies for the current store or channel.

```php
public get_channel_aware_currencies(): array
```

Filters the enabled currencies based on the current channel's allowed currencies.







**Return Value:**

The list of channel-aware currencies.




***


***
> Automatically generated on 2025-01-13
