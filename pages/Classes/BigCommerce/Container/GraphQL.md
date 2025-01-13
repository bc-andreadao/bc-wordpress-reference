***

# GraphQL

This class provides functionality for registering GraphQL-related services, such as various
query objects and a GraphQL requestor processor, in the BigCommerce container. The `register`
method configures these services to be accessed globally through the container.



* Full name: `\BigCommerce\Container\GraphQL`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`GRAPHQL_REQUESTOR`|public|string|&#039;bigcommerce.graphql_requestor&#039;|
|`QUERY`|public|string|&#039;bigcommerce.graphql_query&#039;|
|`PRODUCT_QUERY`|public|string|&#039;bigcommerce.graphql_query_products&#039;|
|`REVIEWS_QUERY`|public|string|&#039;bigcommerce.graphql_query_reviews&#039;|
|`TERMS_QUERY`|public|string|&#039;bigcommerce.graphql_query_terms&#039;|
|`CUSTOMER_QUERY`|public|string|&#039;bigcommerce.graphql_query_customer&#039;|


## Methods


### register

Registers the GraphQL-related services in the container.

```php
public register(\Pimple\Container $container): mixed
```

This method registers the GraphQL queries (products, reviews, terms, customer) and the `GraphQL_Processor`
service that will be used to execute GraphQL requests. These services are registered with specific keys
that can be accessed via the container.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The Pimple container instance used for managing dependencies. |





***


***
> Automatically generated on 2025-01-13
