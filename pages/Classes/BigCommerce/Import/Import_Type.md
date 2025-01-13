***

# Import_Type





* Full name: `\BigCommerce\Import\Import_Type`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`IMPORT_TYPE`|public| |&#039;bigcommerce_import_type&#039;|
|`IMPORT_TYPE_FULL`|public| |&#039;import_type_full&#039;|
|`IMPORT_TYPE_PARTIAL`|public| |&#039;import_type_partial&#039;|


## Methods


### __construct

Import_Type constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\CatalogApi $catalog): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$catalog` | **\BigCommerce\Api\v3\Api\CatalogApi** | The Catalog API connection to use for the import |





***

### fetch_modified_product_ids



```php
public fetch_modified_product_ids(): array
```












***

### filter_task_list

Filter task list for partial imports

```php
public filter_task_list(array $task_list): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$task_list` | **array** |  |





***

### is_traditional_import

Check if import is traditional e.g store products on WP side

```php
public static is_traditional_import(): bool
```



* This method is **static**.








***


***
> Automatically generated on 2025-01-13
