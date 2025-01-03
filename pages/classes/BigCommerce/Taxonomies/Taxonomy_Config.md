***

# Taxonomy_Config





* Full name: `\BigCommerce\Taxonomies\Taxonomy_Config`
* This class is an **Abstract class**



## Properties


### taxonomy



```php
protected string $taxonomy
```







***

### post_types



```php
protected array $post_types
```







***

## Methods


### __construct



```php
public __construct(string $taxonomy, array $post_types): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$taxonomy` | **string** | The ID of the taxonomy |
| `$post_types` | **array** | An array of post types that will use this taxonomy |





***

### register

Hook into WordPress to register the taxonomy

```php
public register(): mixed
```












***

### taxonomy



```php
public taxonomy(): string
```









**Return Value:**

The ID of the taxonomy




***

### post_types



```php
public post_types(): array
```









**Return Value:**

The IDs of the post types associated with this taxonomy




***

### get_args

Arguments to pass when registering the taxonomy.

```php
public get_args(): array
```

Filterable with register_taxonomy_args


* This method is **abstract**.







**See Also:**

* \BigCommerce\Taxonomies\register_taxonomy() - for accepted args.

***

### get_labels

Get labels for the taxonomy.

```php
public get_labels(): array
```

Filterable with taxonomy_labels_{$taxonomy_name}


* This method is **abstract**.







***

### get_products_slug

Get the products archive slug. We use get_option here
rather than get_post_type() because we're looking for it
to add to taxonomy slugs before the post type has been
registered.

```php
protected get_products_slug(): string
```









**Return Value:**

The slug for the products archive




***

### get_caps



```php
protected get_caps(): mixed
```












***


***
> Automatically generated on 2025-01-03
