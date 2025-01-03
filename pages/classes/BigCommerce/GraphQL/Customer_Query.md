***

# Customer_Query

Handles customer-related GraphQL queries and fragments.



* Full name: `\BigCommerce\GraphQL\Customer_Query`




## Methods


### get_public_wishlist_query

Returns a GraphQL query to fetch public wishlists for a customer based on entity IDs.

```php
public get_public_wishlist_query(): string
```

The query retrieves details such as page information, wishlist items,
and fragments for product data, including images, prices, and options.







**Return Value:**

The GraphQL query string.




***

### get_wishlist_query

Returns a GraphQL query to fetch wishlist data for a customer based on entity IDs.

```php
public get_wishlist_query(): string
```

The query retrieves wishlist details, including product and price information, with the use of image and price fragments.







**Return Value:**

The GraphQL query string.




***

### get_wishlists_query

Returns a GraphQL query to fetch all wishlists for a customer.

```php
public get_wishlists_query(): string
```

The query retrieves basic wishlist details, including entity ID, name,
public status, and associated items.







**Return Value:**

The GraphQL query string.




***


***
> Automatically generated on 2025-01-03
