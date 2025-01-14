***

# Config





* Full name: `\BigCommerce\Post_Types\Sync_Log\Config`
* Parent class: [`\BigCommerce\Post_Types\Post_Type_Config`](./classes/BigCommerce/Post_Types/Post_Type_Config.md)




## Methods


### get_args

Arguments to pass when registering the post type.

```php
public get_args(): array
```

Filterable with register_post_type_args










**See Also:**

* \BigCommerce\Post_Types\Sync_Log\register_post_type() - for accepted args.

***

### get_labels

Get labels for the post type.

```php
public get_labels(): array
```

Filterable with post_type_labels_{$post_type_name}










***


## Inherited methods


### __construct



```php
public __construct(string $post_type): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_type` | **string** | The post type name |





***

### register

Hook into WordPress to register the post type

```php
public register(): mixed
```












***

### post_type



```php
public post_type(): string
```









**Return Value:**

The ID of the post type




***

### get_args

Arguments to pass when registering the post type.

```php
public get_args(): array
```

Filterable with register_post_type_args


* This method is **abstract**.







**See Also:**

* \BigCommerce\Post_Types\register_post_type() - for accepted args.

***

### get_labels

Get labels for the post type.

```php
public get_labels(): array
```

Filterable with post_type_labels_{$post_type_name}


* This method is **abstract**.







***


***
> Automatically generated on 2025-01-14
