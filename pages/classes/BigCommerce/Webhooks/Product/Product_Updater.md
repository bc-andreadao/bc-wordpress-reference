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



## Properties


### catalog



```php
private \BigCommerce\Api\v3\Api\CatalogApi $catalog
```






***

### channels



```php
private \BigCommerce\Api\v3\Api\ChannelsApi $channels
```






***

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

- [`ApiException`](../../Api/v3/ApiException.md)



***

### update_for_channel

Start product update for the specified channel

```php
private update_for_channel(\BigCommerce\Api\v3\Model\Product $product, \WP_Term $channel): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **\BigCommerce\Api\v3\Model\Product** |  |
| `$channel` | **\WP_Term** |  |




**Throws:**

- [`ApiException`](../../Api/v3/ApiException.md)



***

### get_listing_id

Find the listing ID associated with the product

```php
private get_listing_id(int $product_id, \WP_Term $channel): int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **int** |  |
| `$channel` | **\WP_Term** |  |





***


***
> Automatically generated on 2024-12-10
