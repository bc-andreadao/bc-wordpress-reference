***

# Product_Updater

Class Product_Updater

Handles the process of updating products in BigCommerce through webhooks.

This class is responsible for managing the re-import and update of product data
when triggered by a webhook. It interacts with the BigCommerce Catalog and Channels APIs
to retrieve and update product details while ensuring that listing updates or deletions
are temporarily disabled during the process. Additionally, it ensures that updates are
applied to all active channels for a product.

* Full name: `\BigCommerce\Webhooks\Product\Product_Updater`




## Methods


### __construct

Product_Updater constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\CatalogApi $catalog, \BigCommerce\Api\v3\Api\ChannelsApi $channels): mixed
```

Initializes the Product_Updater class with the necessary dependencies to
interact with BigCommerce Catalog and Channels APIs.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$catalog` | **\BigCommerce\Api\v3\Api\CatalogApi** | The Catalog API instance for interacting with product data. |
| `$channels` | **\BigCommerce\Api\v3\Api\ChannelsApi** | The Channels API instance for managing channel-related operations. |





***

### update

Re-import a previously imported product.

```php
public update(int $product_id): void
```

This method handles updating a product based on the given BigCommerce product ID.
It ensures all active channels are updated and skips the update if no channels are active.
Applies temporary filters to prevent unintended listing updates or deletions during the process.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **int** | BigCommerce product ID to update. |




**Throws:**
<p>If the API request for product data fails.</p>

- [`ApiException`](./classes/BigCommerce/Api/v3/ApiException.md)



***


***
> Automatically generated on 2025-01-03
