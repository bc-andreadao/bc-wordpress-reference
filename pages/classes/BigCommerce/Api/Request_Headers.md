***

# Request_Headers

Provides functionality for adding custom headers to API requests, including plugin-specific
information like WordPress version, plugin version, and PHP version.



* Full name: `\BigCommerce\Api\Request_Headers`




## Methods


### add_plugin_info_headers

Add plugin-related information to the request headers.

```php
public add_plugin_info_headers(array $headers): array
```

This method adds additional headers containing details about the client type, client version,
plugin version, and PHP version to the provided headers array.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$headers` | **array** | The existing array of request headers to which plugin info will be added. |


**Return Value:**

The updated array of headers with added plugin information.




***


***
> Automatically generated on 2024-12-10
