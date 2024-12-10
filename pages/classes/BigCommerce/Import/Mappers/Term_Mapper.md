***

# Term_Mapper

This abstract class provides the base functionality for mapping BigCommerce terms to WordPress terms.

It enforces that extending classes set a taxonomy name for mapping. It also provides methods for
mapping BigCommerce term IDs to WordPress term IDs and for checking if a term already exists in WordPress.

* Full name: `\BigCommerce\Import\Mappers\Term_Mapper`
* This class is an **Abstract class**



## Properties


### taxonomy



```php
protected string $taxonomy
```






***

## Methods


### __construct

Term_Mapper constructor.

```php
public __construct(): mixed
```

Ensures that the taxonomy property is set in the extending class.
Throws an exception if the taxonomy is not set.









**Throws:**
<p>If the taxonomy is not set.</p>

- [`RuntimeException`](../../../RuntimeException.md)



***

### map

Map a BigCommerce term ID to the equivalent WordPress term ID.

```php
public map(int $bc_id): int
```

This method checks if a BigCommerce term exists in WordPress and returns the corresponding term ID.
If the term is not found, it returns 0, indicating it hasn't been imported yet.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_id` | **int** | The BigCommerce term ID to map. |


**Return Value:**

The WordPress term ID or 0 if the term is not found.




***

### find_existing_term

Find an already-imported term in the WordPress database.

```php
protected find_existing_term(int $bc_id): int
```

This method checks the WordPress terms table to find a term with a matching BigCommerce ID.
It returns the term ID if found, or 0 if the term is not found.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_id` | **int** | The BigCommerce term ID to search for. |


**Return Value:**

The ID of the found term, or 0 if not found.




***


***
> Automatically generated on 2024-12-10
