***

# Product_Query

Handle product query data and fragments.

This class provides methods to fetch paginated product data, individual product details, and various product-related information
through fragments and query construction.

* Full name: `\BigCommerce\GraphQL\Product_Query`




## Methods


### get_paginated_products_query

Get paginated products query.

```php
public get_paginated_products_query(): string
```

This method constructs a GraphQL query to retrieve a paginated list of products.







**Return Value:**

The GraphQL query string for paginated products.




***

### get_product_paginated_request_full

Get full paginated product request query with locale.

```php
public get_product_paginated_request_full(): string
```

This method constructs a GraphQL query to retrieve a paginated list of products, including locale information.







**Return Value:**

The full GraphQL query string for paginated products with locale.




***

### get_product_query

Get product query for a specific product by path.

```php
public get_product_query(): string
```

This method constructs a GraphQL query to retrieve a single product based on its path.







**Return Value:**

The GraphQL query string for fetching a specific product by path.




***

### get_product_fragment

Get the product fragment used in queries.

```php
public get_product_fragment(): string
```

This method provides a fragment that defines the structure of a product object in GraphQL queries.







**Return Value:**

The GraphQL fragment for product details.




***

### get_product_info_fragment

Return product info query fragment.

```php
public get_product_info_fragment(): string
```

This method returns the GraphQL fragment that includes product information like name, SKU, and pricing.







**Return Value:**

The GraphQL fragment for product info.




***

### get_product_prices_fragment

Get product prices fragment.

```php
public get_product_prices_fragment(): string
```

This method returns a fragment that defines the pricing structure for products in GraphQL queries.







**Return Value:**

The GraphQL fragment for product prices.




***

### get_multiple_choice_options_fragment

Get multiple choice options fragment.

```php
public get_multiple_choice_options_fragment(): string
```

This method returns a fragment defining multiple choice options available for the product in GraphQL queries.







**Return Value:**

The GraphQL fragment for multiple choice options.




***

### get_swatch_options_fragment

Get swatch options fragment.

```php
public get_swatch_options_fragment(): string
```

This method returns a fragment that defines the swatch options available for the product.







**Return Value:**

The GraphQL fragment for swatch options.




***

### get_product_picklist_fragment

Get product picklist fragment.

```php
public get_product_picklist_fragment(): string
```

This method returns a fragment that defines the product picklist options available for the product.







**Return Value:**

The GraphQL fragment for product picklist options.




***

### get_checkbox_option_fragment

Get checkbox option fragment.

```php
public get_checkbox_option_fragment(): string
```

This method returns a fragment that defines the checkbox options available for the product.







**Return Value:**

The GraphQL fragment for checkbox options.




***


***
> Automatically generated on 2025-01-03
