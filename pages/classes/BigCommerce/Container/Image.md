***

# Image

This class provides functionality for registering image-related services and hooks related to
image import and CDN management within the BigCommerce container. It includes hooks that
determine if image import is allowed and modify image HTML to load images from a CDN if applicable.



* Full name: `\BigCommerce\Container\Image`
* Parent class: [`Provider`](./Provider.md)




## Methods


### register

Registers image import and CDN-related filters.

```php
public register(\Pimple\Container $container): mixed
```

This method registers two filters:
- A filter that checks if image import is allowed.
- A filter that modifies image HTML to load images from CDN if a valid BigCommerce ID is found.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The Pimple container instance used for managing dependencies. |





***


***
> Automatically generated on 2024-12-10
