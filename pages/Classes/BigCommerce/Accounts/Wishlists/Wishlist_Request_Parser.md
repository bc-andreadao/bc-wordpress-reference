***

# Wishlist_Request_Parser

Class Wishlist_Request_Parser

This class parses and processes wishlist-related requests, such as filtering
the product archive to display wishlist items. It integrates with the BigCommerce
Wishlists API to fetch and handle wishlist data and applies necessary filters
and actions to the WordPress environment.

* Full name: `\BigCommerce\Accounts\Wishlists\Wishlist_Request_Parser`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`LIST_PARAM`|public|string|&#039;list&#039;|
|`TOKEN_PARAM`|public|string|&#039;token&#039;|


## Methods


### __construct

Constructor for Wishlist_Request_Parser.

```php
public __construct(\BigCommerce\Api\v3\Api\WishlistsApi $wishlists): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wishlists` | **\BigCommerce\Api\v3\Api\WishlistsApi** | The Wishlists API instance for fetching wishlist data. |





***

### setup_wishlist_request

Setup the wishlist request.

```php
public setup_wishlist_request(\WP $wp): mixed
```

Determines whether the current request is a wishlist request. If so, it fetches the
wishlist data and applies appropriate actions and filters to render the wishlist.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wp` | **\WP** | The WordPress request object. |





***


***
> Automatically generated on 2025-01-14
