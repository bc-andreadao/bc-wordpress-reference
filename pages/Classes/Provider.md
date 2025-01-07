***

# Provider

This abstract class implements the `ServiceProviderInterface` from Pimple. It provides functionality for managing
callback registrations and offers a mechanism to access callbacks dynamically through the `__get` magic method.

Subclasses are expected to define their own service registration logic.

* Full name: `\Provider`
* This class implements:
[`\ServiceProviderInterface`](./classes/ServiceProviderInterface.md)
* This class is an **Abstract class**



## Properties


### callbacks



```php
protected array $callbacks
```







***

## Methods


### __get

Magic method to retrieve registered callbacks by their identifier.

```php
public __get(string $property): callable|null
```

This method allows access to the registered callbacks using property syntax. If the requested property is found
in the `$callbacks` array, it returns the corresponding callback; otherwise, it returns `null`.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$property` | **string** | The identifier of the callback to retrieve. |


**Return Value:**

The registered callback, or `null` if not found.




***

### create_callback

Creates and registers a callback for a specific identifier.

```php
protected create_callback(string $identifier, callable $callback): callable
```

This method ensures that a callback is not already registered under the same identifier. If the identifier is
already in use, an exception is thrown. Otherwise, it adds the callback to the `$callbacks` array.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$identifier` | **string** | The unique identifier for the callback. |
| `$callback` | **callable** | The callback function to register. |


**Return Value:**

The registered callback.



**Throws:**
<p>If the identifier is already in use.</p>

- [`InvalidArgumentException`](./classes/InvalidArgumentException.md)



***


***
> Automatically generated on 2025-01-07
