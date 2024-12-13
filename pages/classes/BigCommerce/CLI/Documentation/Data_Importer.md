***

# Data_Importer

Extends WP_Parser's Importer class to modify the import behavior for class methods and hooks.



* Full name: `\BigCommerce\CLI\Documentation\Data_Importer`
* Parent class: [`Importer`](./classes/WP_Parser/Importer.md)




## Methods


### import_method

Create a post for a class method, selectively importing hooks for protected or private methods.

```php
protected import_method(array $data, int $parent_post_id, bool $import_ignored = false): bool|int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **array** | The method data to import. |
| `$parent_post_id` | **int** | Optional; post ID of the parent (class) this<br />method belongs to. Defaults to zero (no parent). |
| `$import_ignored` | **bool** | Optional; if true, functions marked `@ignore`<br />will also be imported. Defaults to false. |


**Return Value:**

Post ID of the method if successfully imported, false otherwise.




***


***
> Automatically generated on 2024-12-13
