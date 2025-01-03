***

# Missing_Wishlist

Class Missing_Wishlist

Handle missing wishlist page and results message

* Full name: `\BigCommerce\Accounts\Wishlists\Missing_Wishlist`
* Parent class: [`\BigCommerce\Accounts\Wishlists\Wishlist_Public_View`](./classes/BigCommerce/Accounts/Wishlists/Wishlist_Public_View.md)




## Methods


### filter_main_query

Set the query to only show products in the wishlist

```php
public filter_main_query(\WP_Query $query): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$query` | **\WP_Query** |  |





***

### set_page_title

Set the page title to the name of the wishlist

```php
public set_page_title(array $template_data): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$template_data` | **array** |  |





***

### set_wp_title

Filter the wp_title() for the Wish List page

```php
public set_wp_title(string $title, string $post_type): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$title` | **string** |  |
| `$post_type` | **string** |  |





***

### set_no_results_message

Set the No Results message to be wishlist-relevant

```php
public set_no_results_message(array $template_data): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$template_data` | **array** |  |





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
> Automatically generated on 2025-01-03
