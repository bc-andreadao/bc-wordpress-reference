***

# Brand_Mapper

This class is responsible for mapping the BigCommerce brand data to a WordPress term.

It extends the Term_Mapper class and specifies the taxonomy used for the brand mapping.

* Full name: `\BigCommerce\Import\Mappers\Brand_Mapper`
* Parent class: [`\BigCommerce\Import\Mappers\Term_Mapper`](./classes/BigCommerce/Import/Mappers/Term_Mapper.md)



## Properties


### taxonomy



```php
protected string $taxonomy
```







***



## Inherited methods


### __construct

Term_Mapper constructor.

```php
public __construct(): mixed
```

Ensures that the taxonomy property is set in the extending class.
Throws an exception if the taxonomy is not set.









**Throws:**
<p>If the taxonomy is not set.</p>

- [`RuntimeException`](./classes/RuntimeException.md)



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
> Automatically generated on 2024-12-31
