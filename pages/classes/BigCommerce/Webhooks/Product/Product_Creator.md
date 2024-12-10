***

# Product_Creator

Handles the creation of a new product from BigCommerce via webhooks.

This includes fetching product data, managing channel connections, and triggering imports.

* Full name: `\BigCommerce\Webhooks\Product\Product_Creator`



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

### handle_product_creation

Check if channel exists, adds listings to product and start product import

```php
private handle_product_creation(mixed $product, \WP_Term $channel): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **mixed** |  |
| `$channel` | **\WP_Term** |  |





***

### do_import

Run product import

```php
private do_import(mixed $product, mixed $listing, mixed $channel): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **mixed** |  |
| `$listing` | **mixed** |  |
| `$channel` | **mixed** |  |





***

### create_new_product_listings

Create new Listing for the product. By default, listing doesn't exist on the product

```php
private create_new_product_listings(mixed $product, mixed $channel_id): \BigCommerce\Api\v3\Model\ListingCollectionResponse
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product` | **mixed** |  |
| `$channel_id` | **mixed** |  |




**Throws:**

- [`ApiException`](../../Api/v3/ApiException.md)



***


***
> Automatically generated on 2024-12-10
