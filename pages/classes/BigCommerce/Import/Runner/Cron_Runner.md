***

# Cron_Runner





* Full name: `\BigCommerce\Import\Runner\Cron_Runner`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`START_CRON`|public| |&#039;bigcommerce_start_import&#039;|
|`CONTINUE_CRON`|public| |&#039;bigcommerce_continue_import&#039;|


## Methods


### start_import



```php
public start_import(): void
```












***

### continue_import



```php
public continue_import(): void
```












***

### ajax_continue_import

When an ajax request to get the current import status comes in,
run the next step in the process by triggering the scheduled
cron job.

```php
public ajax_continue_import(): void
```

Runs at priority 5, before the ajax response handler










***


***
> Automatically generated on 2024-12-31
