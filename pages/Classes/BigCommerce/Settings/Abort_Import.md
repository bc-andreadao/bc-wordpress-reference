***

# Abort_Import





* Full name: `\BigCommerce\Settings\Abort_Import`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ABORT_IMPORT_OPTION`|public| |&#039;bigcommerce_abort_import_option&#039;|

## Properties


### screen_settings



```php
protected $screen_settings
```







***

## Methods


### __construct



```php
public __construct(mixed $screen_settings): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$screen_settings` | **mixed** |  |





***

### abort

Abort import process, make cleanup and set self::ABORT_IMPORT_OPTION option in order
to detect on next stages that import was aborted

```php
public abort(\BigCommerce\Import\Processors\Cleanup $cleanup): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$cleanup` | **\BigCommerce\Import\Processors\Cleanup** |  |





***


## Inherited methods


### get_option



```php
protected get_option(string $option, bool $default = false): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **string** |  |
| `$default` | **bool** |  |





***

### update_option



```php
protected update_option(string $option, mixed $value, bool $autoload = false): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **string** |  |
| `$value` | **mixed** |  |
| `$autoload` | **bool** |  |





***

### add_option



```php
protected add_option(string $option, mixed $value, bool $autoload = false): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **string** |  |
| `$value` | **mixed** |  |
| `$autoload` | **bool** |  |





***

### delete_option



```php
protected delete_option(string $option): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **string** |  |





***


***
> Automatically generated on 2025-01-07
