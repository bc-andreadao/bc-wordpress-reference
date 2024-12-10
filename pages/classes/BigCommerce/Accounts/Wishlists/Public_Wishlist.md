***

# Public_Wishlist

This class handles the public-facing wishlist view, including customizing the query
to show only products in the wishlist, setting the page title, customizing the
`wp_title()` function, and managing the "No Results" message on the wishlist page.



* Full name: `\BigCommerce\Accounts\Wishlists\Public_Wishlist`
* Parent class: [`\BigCommerce\Accounts\Wishlists\Wishlist_Public_View`](./Wishlist_Public_View.md)



## Properties


### wishlist



```php
private \BigCommerce\Accounts\Wishlists\Wishlist $wishlist
```






***

## Methods


### __construct

Public_Wishlist constructor.

```php
public __construct(\BigCommerce\Accounts\Wishlists\Wishlist $wishlist): mixed
```

Initializes the Public_Wishlist class with the provided Wishlist object, which represents
the user's wishlist and is used throughout the public wishlist view to display wishlist items
and handle related operations.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wishlist` | **\BigCommerce\Accounts\Wishlists\Wishlist** | The Wishlist object associated with the user&#039;s wishlist. |





***

### filter_main_query

Set the query to only show products in the wishlist.

```php
public filter_main_query(\WP_Query $query): void
```

This method customizes the main WordPress query to only return products that are part of the
user's wishlist. If the wishlist is empty, it modifies the query to exclude any results.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** | The WordPress query object. |





***

### set_page_title

Set the page title to the name of the wishlist.

```php
public set_page_title(array $template_data): array
```

This method modifies the page title template data to include the name of the wishlist
in the title of the product archive page.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$template_data` | **array** | The template data for the product archive page. |


**Return Value:**

The modified template data with the updated page title.




***

### set_wp_title

Filter the wp_title() for the Wish List page.

```php
public set_wp_title(string $title, string $post_type): string
```

This method filters the title of the wish list page to include the name of the wishlist.
It modifies the default `wp_title()` function output for product archive pages.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$title` | **string** | The current title. |
| `$post_type` | **string** | The post type for the page. |


**Return Value:**

The modified title.




***

### set_no_results_message

Set the No Results message to be wishlist-relevant.

```php
public set_no_results_message(array $template_data): array
```

This method customizes the "No Results" message when the wishlist is empty. It updates the
template data to show a relevant message and a "Shop Around" button instead of the default
message when no products are found in the wishlist.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$template_data` | **array** | The template data for the &quot;No Results&quot; page. |


**Return Value:**

The modified template data with the updated message and button label.




***


## Inherited methods


### filter_main_query

Filter the main query to display wishlist-specific products.

```php
public filter_main_query(\WP_Query $query): void
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** | The WordPress query object. |





***

### set_page_title

Set the page title for the wishlist view.

```php
public set_page_title(array $template_data): array
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$template_data` | **array** | The template data for the current page. |


**Return Value:**

The modified template data.




***

### set_wp_title

Set the WordPress title for the wishlist page.

```php
public set_wp_title(string $title, string $post_type): string
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$title` | **string** | The current title of the page. |
| `$post_type` | **string** | The type of post being queried. |


**Return Value:**

The modified page title.




***

### set_no_results_message

Set the no results message for the wishlist page.

```php
public set_no_results_message(array $template_data): array
```




* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$template_data` | **array** | The template data for the current page. |


**Return Value:**

The modified template data with updated no results message.




***

### remove_refinery

Remove the refinery component from the product archive template.

```php
public remove_refinery(array $template_data): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$template_data` | **array** | The template data for the current page. |


**Return Value:**

The modified template data with the refinery component removed.




***


***
> Automatically generated on 2024-12-10
