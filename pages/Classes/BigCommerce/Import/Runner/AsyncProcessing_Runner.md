***

# AsyncProcessing_Runner

Handles asynchronous processing for BigCommerce import operations.

This class manages parallel processing of time-consuming import tasks
such as fetching listings, initializing channels, and product fetching.
It implements locking mechanisms to prevent concurrent processing conflicts
and validates processing status to ensure only allowed operations run in parallel.

* Full name: `\BigCommerce\Import\Runner\AsyncProcessing_Runner`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`CONTINUE_IMPORT`|public| |&#039;bigcommerce_async_import_continue&#039;|


## Methods


### run

Perform additional 'bigcommerce/import/run' action in order to speed up import process

```php
public run(): mixed
```












***


***
> Automatically generated on 2025-01-21
