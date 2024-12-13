***

# Product_Importer

Handles the import of a product from BigCommerce to WordPress.



* Full name: `\BigCommerce\Import\Importers\Products\Product_Importer`




## Methods


### __construct

Product_Importer constructor.

```php
public __construct(\BigCommerce\Api\v3\Model\Product $product, \BigCommerce\Api\v3\Model\Listing $listing, \BigCommerce\Api\v3\Api\CatalogApi $catalog_api, \WP_Term $channel_term): mixed
```

Initializes the product importer with relevant product, listing, catalog API, and channel term data.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Api\v3\Model\Product** | The product data from the BigCommerce catalog API. |
| `$listing` | **\BigCommerce\Api\v3\Model\Listing** | The channel listing data from BigCommerce. |
| `$catalog_api` | **\BigCommerce\Api\v3\Api\CatalogApi** | The Catalog API instance for product management. |
| `$channel_term` | **\WP_Term** | The WordPress term representing the product&#039;s channel. |





***

### import

Initiates the import process for the product.

```php
public import(): int
```

Creates the appropriate strategy for importing the product and executes it.







**Return Value:**

The ID of the imported WordPress post.




***


***
> Automatically generated on 2024-12-13
