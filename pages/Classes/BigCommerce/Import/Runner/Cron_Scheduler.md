***

# Cron_Scheduler

Handles scheduling of import tasks using WordPress cron system.

This class is responsible for managing the timing and frequency of BigCommerce
product imports. It handles both the scheduling of new import cycles based on
configured frequency settings and the scheduling of individual batch processes
within an ongoing import.

* Full name: `\BigCommerce\Import\Runner\Cron_Scheduler`




## Methods


### schedule_next_import

Schedule a cron to start the next import

```php
public schedule_next_import(): void
```












***

### schedule_next_batch

Schedule a cron to start the next phase of the current import

```php
public schedule_next_batch(): void
```












***


***
> Automatically generated on 2025-01-21
