***

# Configuration

Extends the base Configuration class to provide additional
functionality, such as filtering default headers for BigCommerce API requests.

This class allows developers to modify API behavior through WordPress filters.

* Full name: `\BigCommerce\Api\Configuration`
* Parent class: [`Configuration`](./classes/BigCommerce/Api/v3/Configuration.md)




## Methods


### getDefaultHeaders

Retrieves the default headers for API requests.

```php
public getDefaultHeaders(): array
```

Allows modification of the headers via the `bigcommerce/api/default_headers` WordPress filter.







**Return Value:**

An array of default headers to be included with API requests.




***


***
> Automatically generated on 2025-01-13
