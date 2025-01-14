***

# Reviews_Table

Class Reviews_Table



* Full name: `\BigCommerce\Schema\Reviews_Table`
* Parent class: [`\BigCommerce\Schema\Table_Maker`](./classes/BigCommerce/Schema/Table_Maker.md)
* **Warning:** this class is **deprecated**. This means that this class will likely be removed in a future version.


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;bc_reviews&#039;|

## Properties


### schema_version



```php
protected $schema_version
```







***

### tables



```php
protected array $tables
```







***

## Methods


### register_tables

Override for the table registration,
as it was removed in version 4.0

```php
public register_tables(): void
```












***

### get_table_definition



```php
protected get_table_definition(mixed $table): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$table` | **mixed** | The name of the table |


**Return Value:**

The CREATE TABLE statement, suitable for passing to dbDelta




***


## Inherited methods


### schema_update_required

Determine if the database schema is out of date
by comparing the integer found in $this->schema_version
with the option set in the WordPress options table

```php
protected schema_update_required(): bool
```












***

### mark_schema_update_complete

Update the option in WordPress to indicate that
our schema is now up to date

```php
protected mark_schema_update_complete(): void
```












***

### register_tables

Register tables with WordPress, and create them if needed

```php
public register_tables(): void
```












***

### get_table_definition



```php
protected get_table_definition(string $table): string
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$table` | **string** | The name of the table |


**Return Value:**

The CREATE TABLE statement, suitable for passing to dbDelta




***

### get_full_table_name



```php
protected get_full_table_name(string $table): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$table` | **string** |  |


**Return Value:**

The full name of the table, including the
table prefix for the current blog




***


***
> Automatically generated on 2025-01-14
