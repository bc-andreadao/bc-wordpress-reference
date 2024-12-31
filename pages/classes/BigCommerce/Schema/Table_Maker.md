***

# Table_Maker

Class Table_Maker

Utility class for creating/updating custom tables

* Full name: `\BigCommerce\Schema\Table_Maker`
* Parent class: [`\BigCommerce\Schema\Schema`](./classes/BigCommerce/Schema/Schema.md)
* This class is an **Abstract class**



## Properties


### tables



```php
protected array $tables
```







***

## Methods


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


***
> Automatically generated on 2024-12-31
