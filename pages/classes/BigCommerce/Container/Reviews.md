***

# Reviews

Provides functionality for managing reviews in the BigCommerce container.

Registers services for handling review-related operations, including caching,
fetching, and product updates.

* Full name: `\BigCommerce\Container\Reviews`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`PRODUCT_LISTENER`|public|string|&#039;reviews.product_listener&#039;|
|`FETCHER`|public|string|&#039;reviews.fetcher&#039;|
|`CACHER`|public|string|&#039;reviews.cacher&#039;|


## Methods


### register

Registers review-related services in the container.

```php
public register(\Pimple\Container $container): mixed
```

Services include:
- Product update listener for tracking metadata changes.
- Review fetcher for retrieving reviews from the API.
- Review cache for caching reviews and updating the cache on product updates.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The DI container for registering services. |





***


***
> Automatically generated on 2025-01-03
