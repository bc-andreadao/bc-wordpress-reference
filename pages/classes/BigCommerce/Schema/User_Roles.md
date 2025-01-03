***

# User_Roles





* Full name: `\BigCommerce\Schema\User_Roles`
* Parent class: [`\BigCommerce\Schema\Schema`](./classes/BigCommerce/Schema/Schema.md)



## Properties


### schema_version



```php
protected int $schema_version
```







***

## Methods


### __construct



```php
public __construct(array $roles): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$roles` | **array** |  |





***

### register_roles

Register tables with WordPress, and create them if needed

```php
public register_roles(): void
```












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
> Automatically generated on 2025-01-03
