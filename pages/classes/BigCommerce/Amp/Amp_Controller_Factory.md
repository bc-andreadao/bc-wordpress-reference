***

# Amp_Controller_Factory

Class Amp_Controller_Factory

Overrides the template controller factory to replace default
template controllers with AMP-specific counterparts when required.

* Full name: `\BigCommerce\Amp\Amp_Controller_Factory`
* Parent class: [`\BigCommerce\Templates\Controller_Factory`](../Templates/Controller_Factory.md)



## Properties


### override_class_map

Mapping of standard template classes to their AMP-specific counterparts.

```php
private array&lt;string,string&gt; $override_class_map
```

This array is used to override the default template controllers with
AMP-compatible versions. Keys are the fully-qualified names of the standard
classes, and values are the corresponding AMP class names.




***

## Methods


### get_controller

Retrieves the appropriate controller for a given class name.

```php
public get_controller(string $classname, array $options = [], string $template = &#039;&#039;): object
```

Overrides the default behavior by replacing the standard class name with
its AMP counterpart if defined in the `$override_class_map`.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$classname` | **string** | Fully-qualified class name of the controller. |
| `$options` | **array** | Optional parameters passed to the controller. |
| `$template` | **string** | Optional template name to associate with the controller. |


**Return Value:**

The controller instance.




***


## Inherited methods


### get_controller

Creates an instance of the requested controller

```php
public get_controller(string $classname, array $options = [], string $template = &#039;&#039;): \BigCommerce\Templates\Controller
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$classname` | **string** |  |
| `$options` | **array** |  |
| `$template` | **string** |  |





***


***
> Automatically generated on 2024-12-10