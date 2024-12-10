***

# Templates

Handles template overrides and body class modifications
within the BigCommerce integration. It registers various filters to modify the template paths and
the body class dynamically based on the context, such as product pages, archives, taxonomies, and search results.



* Full name: `\BigCommerce\Container\Templates`
* Parent class: [`Provider`](./Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`OVERRIDE`|public|string|&#039;template.override&#039;|
|`BODY_CLASS`|public|string|&#039;template.body_class&#039;|


## Methods


### register

Register the template-related services and filters.

```php
public register(\Pimple\Container $container): mixed
```

This method registers all the necessary services and filters related to templates, including
template overrides, body classes, and template hierarchy modifications. It is called when the
container is initialized and hooks into various WordPress actions and filters for template management.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The container instance used to register services. |





***


***
> Automatically generated on 2024-12-10
