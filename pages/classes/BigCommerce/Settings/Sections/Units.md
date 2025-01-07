***

# Units

Class Units

May eventually expose UI for these settings, but for now
they are imported from the BigCommerce API and not exposed
in the admin.

* Full name: `\BigCommerce\Settings\Sections\Units`
* Parent class: [`\BigCommerce\Settings\Sections\Settings_Section`](./classes/BigCommerce/Settings/Sections/Settings_Section.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`MASS`|public| |&#039;bigcommerce_mass_unit&#039;|
|`LENGTH`|public| |&#039;bigcommerce_length_unit&#039;|
|`POUND`|public| |&#039;lb&#039;|
|`OUNCE`|public| |&#039;oz&#039;|
|`KILOGRAM`|public| |&#039;kg&#039;|
|`GRAM`|public| |&#039;g&#039;|
|`TONNE`|public| |&#039;tonne&#039;|
|`INCH`|public| |&#039;in&#039;|
|`CENTIMETER`|public| |&#039;cm&#039;|




## Inherited methods


### render_field



```php
public render_field(array $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** |  |





***

### render_number_field



```php
public render_number_field(array $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** |  |





***

### get_disabled_attr_headless

Get disabled attribute if headless option is on

```php
public get_disabled_attr_headless(): string
```












***


***
> Automatically generated on 2025-01-07
