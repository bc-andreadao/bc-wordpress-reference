***

# Rewrites

Handles rewrite rules and flushing mechanisms for the BigCommerce container.

Registers services and hooks to manage custom rewrite rules, flushing
permalinks, and handling requests via custom endpoints.

* Full name: `\BigCommerce\Container\Rewrites`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION_ENDPOINT`|public|string|&#039;rewrites.action_endpoint&#039;|
|`FLUSH`|public|string|&#039;rewrites.flush&#039;|


## Methods


### register

Registers rewrite-related services and hooks in the container.

```php
public register(\Pimple\Container $container): mixed
```

Services include:
- Action endpoint for managing custom route registration and requests.
- Flusher for handling permalink flush operations.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The DI container for registering services. |





***


***
> Automatically generated on 2025-01-13
