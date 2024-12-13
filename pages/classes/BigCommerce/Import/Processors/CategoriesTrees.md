***

# CategoriesTrees

This trait provides methods for working with BigCommerce category trees.

It includes functionality to fetch categories within a specific category tree.

* Full name: `\BigCommerce\Import\Processors\CategoriesTrees`




## Methods


### get_msf_categories

Get the categories in the MSF category tree.

```php
public get_msf_categories(\BigCommerce\Api\v3\Api\CatalogApi $api, array $params = []): \BigCommerce\Api\v3\Model\CategoryCollectionResponse|array
```

This method retrieves categories within the MSF category tree by fetching the tree ID,
then requesting a batch of categories from the BigCommerce API.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api` | **\BigCommerce\Api\v3\Api\CatalogApi** | The BigCommerce Catalog API instance. |
| `$params` | **array** | Additional parameters for the category query (optional). |


**Return Value:**

A collection of categories or an empty array.



**Throws:**
<p>Throws an exception if the API request fails.</p>

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



***

### get_trees

Get all category trees associated with a given channel.

```php
public get_trees(\BigCommerce\Api\v3\Api\CatalogApi $api): array
```

This method fetches category trees from BigCommerce by retrieving the channel ID
associated with the primary connection and querying the BigCommerce API for
available category trees.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api` | **\BigCommerce\Api\v3\Api\CatalogApi** | The BigCommerce Catalog API instance. |


**Return Value:**

An array of category trees.



**Throws:**
<p>Throws an exception if the API request fails.</p>

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



***

***
> Automatically generated on 2024-12-13

