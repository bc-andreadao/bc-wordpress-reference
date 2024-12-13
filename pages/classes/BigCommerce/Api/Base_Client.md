***

# Base_Client

Base API client class that extends the ApiClient and manages the configuration
of the API client. This class is designed to handle the configuration for
API communication and can be extended for specific API clients.



* Full name: `\BigCommerce\Api\Base_Client`
* Parent class: [`ApiClient`](./classes/BigCommerce/Api/v3/ApiClient.md)



## Properties


### config

Configuration for the API client

```php
protected \BigCommerce\Api\Configuration $config
```







***

## Methods


### __construct

Constructor for the Base_Client class

```php
public __construct(\BigCommerce\Api\Configuration|null $config = null): mixed
```

Initializes the API client with the provided configuration. If no configuration
is provided, it will use the default configuration.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **\BigCommerce\Api\Configuration&#124;null** | The configuration for this ApiClient. |





***

### getConfig

Gets the configuration of the API client

```php
public getConfig(): \BigCommerce\Api\Configuration
```

Returns the configuration object used by the API client.







**Return Value:**

Returns the Configuration object used by this API client.




***


***
> Automatically generated on 2024-12-13
