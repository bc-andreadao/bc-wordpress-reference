***

# Product_Ignorer

Strategy for skipping a product during the import process.



* Full name: `\BigCommerce\Import\Importers\Products\Product_Ignorer`
* This class implements:
[`\BigCommerce\Import\Import_Strategy`](./classes/BigCommerce/Import/Import_Strategy.md)




## Methods


### __construct

Product_Ignorer constructor.

```php
public __construct(\BigCommerce\Api\v3\Model\Product $product, \BigCommerce\Api\v3\Model\Listing $listing, \WP_Term $channel_term, \BigCommerce\Api\v3\Api\CatalogApi $catalog, int $post_id): mixed
```

Initializes the product ignorer with relevant data and dependencies.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Api\v3\Model\Product** | The product data. |
| `$listing` | **\BigCommerce\Api\v3\Model\Listing** | The channel listing data. |
| `$channel_term` | **\WP_Term** | The WordPress term representing the channel. |
| `$catalog` | **\BigCommerce\Api\v3\Api\CatalogApi** | The Catalog API instance. |
| `$post_id` | **int** | The WordPress post ID. |





***

### do_import

Skips the import process for the current product.

```php
public do_import(): int
```

Triggers a custom action hook for other processes to react to the product being skipped.







**Return Value:**

The WordPress post ID of the skipped product.




***


***
> Automatically generated on 2025-01-03
