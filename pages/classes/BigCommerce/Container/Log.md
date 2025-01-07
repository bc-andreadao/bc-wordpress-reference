***

# Log

This class is responsible for setting up logging functionality in the BigCommerce container.

It registers services for logging, defines constants for log paths, and handles log-related actions
during the BigCommerce import process, such as logging errors and diagnostics.

* Full name: `\BigCommerce\Container\Log`
* Parent class: [`Provider`](./classes/BigCommerce/Container/Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`LOGGER`|public|string|&#039;logger.log&#039;|
|`LOG_PATH`|public|string|&#039;logger.log_path&#039;|
|`LOG_FOLDER_PATH`|public|string|&#039;logger.log_folder_path&#039;|


## Methods


### register

Registers logging-related services and actions in the container.

```php
public register(\Pimple\Container $container): mixed
```

This method sets up the necessary services for logging, such as the log file path,
log folder path, and logger instance. It also registers various actions and filters
for logging during the BigCommerce import process.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The container instance used to register the services. |





***


***
> Automatically generated on 2025-01-07
