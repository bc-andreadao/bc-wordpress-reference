***

# Mini_Cart

Manages the configuration and display logic for the mini-cart widget in BigCommerce.



* Full name: `\BigCommerce\Cart\Mini_Cart`




## Methods


### add_mini_cart_config

Adds mini-cart configuration to the global JavaScript configuration array.

```php
public add_mini_cart_config(array $config): array
```

This method appends the `mini_cart` configuration to the provided configuration array.
It determines whether the mini-cart widget is enabled and passes this value.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **array** | The existing JavaScript configuration array. |


**Return Value:**

The modified configuration array with mini-cart settings.




***

### mini_cart_enabled



```php
private mini_cart_enabled(): mixed
```












***


***
> Automatically generated on 2024-12-10
