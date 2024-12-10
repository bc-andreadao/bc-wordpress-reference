***

# Product_Creator

Handles the creation of a new product from BigCommerce via webhooks.

This includes fetching product data, managing channel connections, and triggering imports.

* Full name: `\BigCommerce\Webhooks\Product\Product_Creator`




## Methods


### __construct

Product_Creator constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\CatalogApi $catalog, \BigCommerce\Api\v3\Api\ChannelsApi $channels): mixed
```

Initializes API clients for catalog and channel operations.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$catalog` | **\BigCommerce\Api\v3\Api\CatalogApi** | Catalog API client. |
| `$channels` | **\BigCommerce\Api\v3\Api\ChannelsApi** | Channels API client. |





***

### create

Creates a new product in BigCommerce.

```php
public create(int $product_id): mixed
```

Handles the entire product creation process, including:
- Fetching the product from the BigCommerce catalog.
- Verifying active channels for product listing.
- Initiating product import workflows.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **int** | The ID of the product to create. |





***


***
> Automatically generated on 2024-12-10
