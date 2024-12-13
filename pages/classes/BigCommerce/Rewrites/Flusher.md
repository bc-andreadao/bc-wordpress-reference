***

# Flusher

Handles flushing and scheduling of WordPress rewrite rules for the BigCommerce plugin.



* Full name: `\BigCommerce\Rewrites\Flusher`




## Methods


### schedule_flush

Schedules a rewrite flush by setting an option to mark rewrites as pending.

```php
public schedule_flush(): void
```

This method updates the `bigcommerce_flushed_rewrites` option to `0`,
signaling that a rewrite flush is required.










***

### do_flush

Executes a rewrite flush if it hasn't been performed yet.

```php
public do_flush(): void
```

This method checks the `bigcommerce_flushed_rewrites` option. If it's not set to `1`,
it flushes the rewrite rules and updates the option to `1`, preventing unnecessary future flushes.

Hook: Triggered on the `wp_loaded` action.










***


***
> Automatically generated on 2024-12-13
