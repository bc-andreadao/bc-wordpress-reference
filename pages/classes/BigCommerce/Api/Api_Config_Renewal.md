***

# Api_Config_Renewal

Class Api_Config_Renewal

Handles the renewal of API configuration settings.

This class is responsible for updating the configuration of the BigCommerce API
based on new credentials (store URL, client ID, client secret, and access token).
After updating the configuration, it reconfigures the BigCommerce API client
with the new credentials.

* Full name: `\BigCommerce\Api\Api_Config_Renewal`




## Methods


### __construct

Api_Config_Renewal constructor.

```php
public __construct(\BigCommerce\Api\Configuration $config): mixed
```

Initializes the API configuration renewal process.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **\BigCommerce\Api\Configuration** | The configuration object used to store and manage API credentials. |





***

### renewal_config

Renews the API configuration based on the provided option and value.

```php
public renewal_config(string $option, string $value): \BigCommerce\Api\Configuration
```

This function updates the API configuration by setting the new value for
the specified option (store URL, client ID, client secret, or access token).
After updating the configuration, it reconfigures the BigCommerce API client
with the new credentials.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$option` | **string** | The configuration option to renew (e.g., &#039;store_url&#039;, &#039;client_id&#039;). |
| `$value` | **string** | The new value for the configuration option. |


**Return Value:**

The updated configuration object.




***


***
> Automatically generated on 2024-12-13
