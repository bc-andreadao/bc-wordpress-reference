***

# Product_Strategy_Factory

Factory class for determining the appropriate import strategy for a product.

This class decides whether to create, ignore, or update a product based on its existence and freshness.

* Full name: `\BigCommerce\Import\Importers\Products\Product_Strategy_Factory`




## Methods


### __construct

Product_Strategy_Factory constructor.

```php
public __construct(\BigCommerce\Api\v3\Model\Product $product, \BigCommerce\Api\v3\Model\Listing $listing, \WP_Term $channel_term, \BigCommerce\Api\v3\Api\CatalogApi $catalog, string $version): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Api\v3\Model\Product** | The product data from BigCommerce API |
| `$listing` | **\BigCommerce\Api\v3\Model\Listing** | The channel listing data from BigCommerce API |
| `$channel_term` | **\WP_Term** | The channel term for the product import |
| `$catalog` | **\BigCommerce\Api\v3\Api\CatalogApi** | The Catalog API instance |
| `$version` | **string** | The version of the importer |





***

### get_strategy

Returns the appropriate import strategy based on the product and channel data.

```php
public get_strategy(): \BigCommerce\Import\Import_Strategy
```









**Return Value:**

The import strategy (either Product_Creator, Product_Ignorer, or Product_Updater)




***


***
> Automatically generated on 2024-12-31
