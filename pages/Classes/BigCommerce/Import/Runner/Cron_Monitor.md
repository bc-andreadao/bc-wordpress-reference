***

# Cron_Monitor

Class Cron_Monitor

Makes sure that the import tasks are scheduled appropriately

* Full name: `\BigCommerce\Import\Runner\Cron_Monitor`




## Methods


### check_for_scheduled_crons



```php
public check_for_scheduled_crons(): void
```












***

### listen_for_changed_schedule



```php
public listen_for_changed_schedule(mixed $old_value, mixed $new_value): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$old_value` | **mixed** |  |
| `$new_value` | **mixed** |  |





***

### listen_for_import_start

If an import is starting, unschedule the next scheduled start.

```php
public listen_for_import_start(mixed $status): void
```

Usually means that an import is running from the CLI.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$status` | **mixed** |  |





***


***
> Automatically generated on 2025-01-14
