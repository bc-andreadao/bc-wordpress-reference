***

# Query_Filter

Class Query_Filter

Responsible for filtering front-end queries to only show
products in the current channel

* Full name: `\BigCommerce\Taxonomies\Channel\Query_Filter`




## Methods


### apply

Filter the query to show products for the current channel

```php
public apply(\WP_Query $query): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** |  |





***

### is_product_archive_query

Determine if the query is for an archive that may include products

```php
private is_product_archive_query(\WP_Query $query): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** |  |





***

### has_channel_filter

Determine if there's already a channel filter at the top level
of the query. This prevents adding a conflicting filter to a request
that's already looking in a specific channel.

```php
private has_channel_filter(\WP_Query $query): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** |  |





**See Also:**

* \BigCommerce\Post_Types\Product\Product::by_product_id() - 

***

### set_tax_query

Set the tax query so that it excludes products in other channels

```php
private set_tax_query(\WP_Query $query, \WP_Term $current_channel): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** |  |
| `$current_channel` | **\WP_Term** |  |





***

### is_singular_product_query

Determine if the query is for a single product

```php
private is_singular_product_query(\WP_Query $query): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** |  |





***

### set_product_query

Set the query so that it selects the correct product with the given slug for the channel

```php
private set_product_query(\WP_Query $query, \WP_Term $current_channel): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** |  |
| `$current_channel` | **\WP_Term** |  |





***


***
> Automatically generated on 2024-12-10
