***

# Term_Strategy_Factory

A factory class that determines the appropriate strategy for handling term imports,
such as creating, updating, or ignoring a term based on its existing data in WordPress.



* Full name: `\BigCommerce\Import\Importers\Terms\Term_Strategy_Factory`



## Properties


### bc_term



```php
private \ArrayAccess $bc_term
```






***

### taxonomy



```php
private string $taxonomy
```






***

## Methods


### __construct

Term_Strategy_Factory constructor.

```php
public __construct(\ArrayAccess $bc_term, string $taxonomy): mixed
```

Initializes the Term_Strategy_Factory with the provided BigCommerce term data and taxonomy.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_term` | **\ArrayAccess** | The BigCommerce term data. |
| `$taxonomy` | **string** | The taxonomy for the term. |





***

### get_strategy

Identifies the appropriate strategy for handling the term import based on existing data in WordPress.

```php
public get_strategy(): \BigCommerce\Import\Import_Strategy
```

The strategy is selected based on whether the term exists and whether it needs to be updated.







**Return Value:**

The selected strategy for handling the term import.




***

### get_matching_term

Find an existing term based on the same BigCommerce product

```php
private get_matching_term(): int
```









**Return Value:**

The WordPress term ID, or 0 if not found




***

### needs_refresh



```php
private needs_refresh(mixed $term_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term_id` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10
