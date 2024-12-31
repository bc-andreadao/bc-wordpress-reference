***

# Term_Saver

Provides functionality for saving terms into WordPress, including term data, term metadata,
and term images. This class implements the Import_Strategy interface, allowing it to be used
within an import process. It contains methods for handling terms in BigCommerce and saving them
in WordPress.



* Full name: `\BigCommerce\Import\Importers\Terms\Term_Saver`
* This class implements:
[`\BigCommerce\Import\Import_Strategy`](./classes/BigCommerce/Import/Import_Strategy.md)
* This class is an **Abstract class**


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`DATA_HASH_META_KEY`|public| |&#039;bigcommerce_data_hash&#039;|
|`IMPORTER_VERSION_META_KEY`|public| |&#039;bigcommerce_importer_version&#039;|

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

Term_Saver constructor.

```php
public __construct(\ArrayAccess $bc_term, string $taxonomy, int $term_id): mixed
```

Initializes the Term_Saver with the provided BigCommerce term, taxonomy, and optional term ID.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_term` | **\ArrayAccess** | The BigCommerce term data. |
| `$taxonomy` | **string** | The taxonomy the term belongs to. |
| `$term_id` | **int** | The term ID in WordPress (default is 0). |





***

### do_import

Imports the term into WordPress, saving term data, term metadata, and images.

```php
public do_import(): int
```









**Return Value:**

The imported term ID.




***

### get_term_bc_id

Returns the BigCommerce ID of the term.

```php
public get_term_bc_id(\ArrayAccess $bc_term): int|null
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_term` | **\ArrayAccess** | The BigCommerce term data. |


**Return Value:**

The BigCommerce ID or category ID.




***

### save_wp_term

Saves the term in WordPress.

```php
protected save_wp_term(\ArrayAccess $bc_term): int
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_term` | **\ArrayAccess** | The BigCommerce term data. |


**Return Value:**

The ID of the created or updated term.




***

### save_wp_termmeta

Saves the term metadata in WordPress.

```php
protected save_wp_termmeta(\ArrayAccess $bc_term): mixed
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_term` | **\ArrayAccess** | The BigCommerce term data. |





***

### term_name

Returns the name of the term, sanitized for WordPress.

```php
protected term_name(\ArrayAccess $bc_term): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_term` | **\ArrayAccess** | The BigCommerce term data. |


**Return Value:**

The sanitized term name.




***

### term_slug

Returns the slug for the term, either from the custom URL or generated from the name.

```php
protected term_slug(\ArrayAccess $bc_term): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_term` | **\ArrayAccess** | The BigCommerce term data. |


**Return Value:**

The term slug.




***

### sanitize_int

Sanitizes an integer value.

```php
protected sanitize_int(mixed $value): int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** | The value to sanitize. |


**Return Value:**

The sanitized integer value.




***

### sanitize_string

Sanitizes a string value.

```php
protected sanitize_string(mixed $value): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** | The value to sanitize. |


**Return Value:**

The sanitized string value.




***

### get_term_args

Returns the arguments for the term, including the slug, description, and parent ID.

```php
protected get_term_args(\ArrayAccess $bc_term): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_term` | **\ArrayAccess** | The BigCommerce term data. |


**Return Value:**

The arguments for the term.




***

### determine_parent_term_id

Determines the parent term ID for the given BigCommerce term.

```php
protected determine_parent_term_id(\ArrayAccess $bc_term): int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_term` | **\ArrayAccess** | The BigCommerce term data. |


**Return Value:**

The parent term ID.




***

### import_image

Imports the image for the term, either by finding an existing image or importing a new one.

```php
protected import_image(\ArrayAccess $bc_term): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_term` | **\ArrayAccess** | The BigCommerce term data. |





***

### hash

Calculates a hash for the given term data.

```php
public static hash(\ArrayAccess $bc_term): string
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_term` | **\ArrayAccess** | The BigCommerce term data. |


**Return Value:**

The calculated hash.




***


***
> Automatically generated on 2024-12-31
