***

# Matomo

This class integrates BigCommerce with Matomo (formerly Piwik), a web analytics platform. It provides functionality for
modifying the JavaScript configuration for tracking user interactions with custom variables in Matomo.

The class specifically hooks into the `bigcommerce/js_config` filter to add custom variables to the JavaScript configuration.

* Full name: `\BigCommerce\Compatibility\Matomo\Matomo`




## Methods


### js_config

Adds custom variables to the JavaScript configuration for Matomo tracking.

```php
public js_config(array $config): array
```

This method hooks into the `bigcommerce/js_config` filter and modifies the configuration array to include Matomo's
custom variables. By default, it includes a custom variable for the BigCommerce channel (BC_Channel), which can be extended
for more custom tracking variables.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **array** | The existing JavaScript configuration array that can be modified. |


**Return Value:**

The modified configuration array with the added Matomo custom variables.




***


***
> Automatically generated on 2025-01-14
