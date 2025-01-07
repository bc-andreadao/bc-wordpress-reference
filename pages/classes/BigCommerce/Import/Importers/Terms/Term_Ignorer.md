***

# Term_Ignorer

Handles the logic for skipping the import of a term in the BigCommerce import process. This class implements
the Import_Strategy interface and provides a method for processing a term that should be ignored.



* Full name: `\BigCommerce\Import\Importers\Terms\Term_Ignorer`
* This class implements:
[`\BigCommerce\Import\Import_Strategy`](./classes/BigCommerce/Import/Import_Strategy.md)



## Properties


### bc_term



```php
protected \ArrayAccess $bc_term
```







***

### taxonomy



```php
protected string $taxonomy
```







***

### term_id



```php
protected int $term_id
```







***

## Methods


### __construct

Term_Ignorer constructor.

```php
public __construct(\ArrayAccess $bc_term, string $taxonomy, int $term_id): mixed
```

Initializes the Term_Ignorer with the provided BigCommerce term, taxonomy, and optional term ID.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_term` | **\ArrayAccess** | The BigCommerce term data. |
| `$taxonomy` | **string** | The taxonomy the term belongs to. |
| `$term_id` | **int** | The WordPress term ID (default is 0). |





***

### do_import

Skips the import of the current term and updates its visibility.

```php
public do_import(): int
```

This method triggers a `do_action` hook indicating the term has been skipped for import
and updates the term's visibility status in WordPress.







**Return Value:**

The term ID after skipping the import.




***


***
> Automatically generated on 2025-01-07
