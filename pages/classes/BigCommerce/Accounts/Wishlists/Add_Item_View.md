***

# Add_Item_View

Class Add_Item_View

Adds the "Add to Wish List" template after the purchase form on the product single view.
This class manages the display of the "Add to Wishlist" button and the wishlist functionality
on product detail pages. It checks whether the feature is enabled, if the user is logged in,
and then allows the user to add a product to an existing wishlist.

* Full name: `\BigCommerce\Accounts\Wishlists\Add_Item_View`



## Properties


### wishlists



```php
private \BigCommerce\Api\v3\Api\WishlistsApi $wishlists
```






***

## Methods


### __construct

Add_Item_View constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\WishlistsApi $wishlists): mixed
```

Initializes the Add_Item_View class with the provided WishlistsApi instance, which is used
to interact with the BigCommerce API to manage wishlists.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wishlists` | **\BigCommerce\Api\v3\Api\WishlistsApi** | The WishlistsApi instance to interact with BigCommerce wishlists. |





***

### filter_product_single_template

Filters the data of the product single template to add the "Add to Wish List" button.

```php
public filter_product_single_template(array $data, string $template, array $options): array
```

This method checks if the "Add to Wishlist" feature is enabled, if the user is logged in,
and if the customer has a wishlist. If all conditions are met, it adds the "Add to Wish List"
button to the product single template.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **array** | The template data for the product single page. |
| `$template` | **string** | The name of the template file. |
| `$options` | **array** | Additional options for rendering the template. |


**Return Value:**

The modified template data with the "Add to Wish List" button included.




***

### get_wishlists

Fetches the customer's wishlists from the API.

```php
private get_wishlists(int $customer_id): \BigCommerce\Accounts\Wishlists\Wishlist[]
```

This method retrieves a list of the customer's existing wishlists and returns them as
an array of Account_Wishlist objects.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$customer_id` | **int** | The ID of the customer to fetch wishlists for. |


**Return Value:**

An array of Account_Wishlist objects representing the customer's wishlists.




***


***
> Automatically generated on 2024-12-10