***

# Wishlist

Class Wishlist

A wrapper around API wishlists to manage wishlist data, generate URLs for wishlist actions,
and handle items in the wishlist.

* Full name: `\BigCommerce\Accounts\Wishlists\Wishlist`




## Methods


### __construct

Wishlist constructor.

```php
public __construct(\BigCommerce\Api\v3\Model\Wishlist $wishlist): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$wishlist` | **\BigCommerce\Api\v3\Model\Wishlist** | The wishlist API model |





***

### list_id

Get the ID of the wishlist.

```php
public list_id(): int
```









**Return Value:**

The ID of the wishlist.




***

### customer_id

Get the customer ID associated with the wishlist.

```php
public customer_id(): int
```









**Return Value:**

The customer ID.




***

### token

Get the token associated with the wishlist.

```php
public token(): string
```









**Return Value:**

The wishlist token.




***

### name

Get the name of the wishlist.

```php
public name(): string
```









**Return Value:**

The name of the wishlist.




***

### count

Get the number of items in the wishlist.

```php
public count(): int
```









**Return Value:**

The number of items.




***

### wishlist

Get the underlying API wishlist object.

```php
public wishlist(): \BigCommerce\Api\v3\Model\Wishlist
```









**Return Value:**

The wishlist API model.




***

### items

Get the product IDs of items in the wishlist.

```php
public items(): int[]
```









**Return Value:**

Array of product IDs.




***

### raw_items

Get the raw item objects from the API response.

```php
public raw_items(): \BigCommerce\Api\v3\Model\WishlistItem[]
```









**Return Value:**

Array of raw wishlist item objects.




***

### is_public

Check if the wishlist is publicly shared.

```php
public is_public(): bool
```









**Return Value:**

True if the wishlist is public, false otherwise.




***

### public_url

Get the public URL to view the wishlist.

```php
public public_url(): string
```









**Return Value:**

The URL to view the wishlist.




***

### user_url

Get the user's private URL to view the wishlist.

```php
public user_url(): string
```









**Return Value:**

The user's private wishlist URL.




***

### edit_url

Get the URL to handle update requests for this wishlist.

```php
public edit_url(): string
```









**Return Value:**

The URL for wishlist updates.




***

### delete_url

Get the URL to delete the wishlist.

```php
public delete_url(): string
```









**Return Value:**

The URL to delete the wishlist.




***

### add_item_url

Get the URL to add an item to the wishlist.

```php
public add_item_url(int $product_id): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **int** | The ID of the product to add. |


**Return Value:**

The URL for adding an item to the wishlist.




***

### delete_item_url

Get the URL to remove an item from the wishlist.

```php
public delete_item_url(int $product_id): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$product_id` | **int** | The ID of the product to remove. |


**Return Value:**

The URL for removing an item from the wishlist.




***

### create_url

Get the URL to create a wishlist.

```php
public static create_url(): string
```



* This method is **static**.





**Return Value:**

The URL to create a new wishlist.




***


***
> Automatically generated on 2025-01-07
