***

# Plugin





* Full name: `\BigCommerce\Plugin`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`VERSION`|public| |&#039;5.1.2&#039;|

## Properties


### _instance



```php
protected static $_instance
```



* This property is **static**.



***

### container



```php
protected \Pimple\Container $container
```







***

## Methods


### __construct



```php
public __construct(\Pimple\Container $container): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** |  |





***

### __get



```php
public __get(mixed $property): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$property` | **mixed** |  |





***

### init



```php
public init(): mixed
```












***

### container



```php
public container(): mixed
```












***

### plugin_dir_url



```php
public plugin_dir_url(): string
```









**Return Value:**

The URL for the plugin's root directory, with a trailing slash




***

### plugin_dir_path



```php
public plugin_dir_path(): string
```









**Return Value:**

The file system path for the plugin's root directory, with a trailing slash




***

### credentials_set

Determines is API credentials have been set, a prerequisite
for much of the plugin functionality.

```php
public credentials_set(): bool
```












***

### instance



```php
public static instance(null|\ArrayAccess $container = null): self
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **null&#124;\ArrayAccess** |  |




**Throws:**

- [`Exception`](./classes/Exception.md)



***

### activate



```php
public static activate(): mixed
```



* This method is **static**.








***


***
> Automatically generated on 2025-01-14
