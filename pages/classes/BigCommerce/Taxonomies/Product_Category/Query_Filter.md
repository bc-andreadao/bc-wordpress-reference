***

# Query_Filter





* Full name: `\BigCommerce\Taxonomies\Product_Category\Query_Filter`




## Methods


### __construct



```php
public __construct(\BigCommerce\Taxonomies\Product_Category\Group_Filtered_Terms $group_filtered_terms): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$group_filtered_terms` | **\BigCommerce\Taxonomies\Product_Category\Group_Filtered_Terms** |  |





***

### apply

Filter the query to show products for the whitelisted product categories

```php
public apply(\WP_Query $query): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** |  |





***

### get_non_visible_terms

Retrieve a list of terms with is_visible = false

```php
public get_non_visible_terms(): array
```












***

### maybe_hide_children

When retrieving a term that has children, WP will include the children in the archive unless we specifically
exclude it. This only applies when a group has visibility of a parent term, but not children.

```php
public maybe_hide_children(mixed $query): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **mixed** |  |





***


***
> Automatically generated on 2024-12-31
