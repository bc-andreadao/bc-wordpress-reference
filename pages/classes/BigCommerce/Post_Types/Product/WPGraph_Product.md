***

# WPGraph_Product





* Full name: `\BigCommerce\Post_Types\Product\WPGraph_Product`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`SINGULAR`|public| |&#039;BCProduct&#039;|
|`PLURAL`|public| |&#039;BCProducts&#039;|

## Properties


### config



```php
private $config
```






***

## Methods


### __construct



```php
public __construct(\BigCommerce\Post_Types\Product\WPGraph_Config $config): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **\BigCommerce\Post_Types\Product\WPGraph_Config** |  |





***

### register



```php
public register(): mixed
```












***

### register_field_types

Add support for collection fields like BCVariants and BCVariantsOptions

```php
protected register_field_types(): void
```












***

### register_product_properties

Process single product and register fields for it

```php
protected register_product_properties(): void
```












***

### register_variants

Register variants collection field

```php
protected register_variants(): void
```












***

### register_variants_options

Register single variant option values field and tie it to the BCVariants field

```php
protected register_variants_options(): void
```












***

### register_fields



```php
private register_fields(array $source = []): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$source` | **array** |  |





***

### get_variants_options_args



```php
private get_variants_options_args(): array
```












***

### get_variants_fields_args



```php
private get_variants_fields_args(): array
```












***


***
> Automatically generated on 2024-12-10
