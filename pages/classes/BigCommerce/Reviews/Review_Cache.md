***

# Review_Cache

Class Review_Cache

Caches the first page of a product's reviews in post meta

* Full name: `\BigCommerce\Reviews\Review_Cache`



## Properties


### fetcher



```php
private \BigCommerce\Reviews\Review_Fetcher $fetcher
```






***

## Methods


### __construct



```php
public __construct(\BigCommerce\Reviews\Review_Fetcher $fetcher): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$fetcher` | **\BigCommerce\Reviews\Review_Fetcher** |  |





***

### update_cache



```php
public update_cache(int $product_id): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **int** |  |





***

### get_matching_imported_products

We only want to import reviews if we have a product
imported into the database corresponding to those
reviews. If the product is disabled for all active
channels, we skip the review import.

```php
private get_matching_imported_products(int $product_id): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **int** | The BigCommerce product ID |


**Return Value:**

The post IDs related to the product ID for all channels




***


***
> Automatically generated on 2024-12-10
