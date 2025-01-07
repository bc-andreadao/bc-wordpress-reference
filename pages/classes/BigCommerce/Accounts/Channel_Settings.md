***

# Channel_Settings

Manages channel settings related to global logins, syncing customer settings,
and scheduling resyncs for updated global login configurations.



* Full name: `\BigCommerce\Accounts\Channel_Settings`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`RESYNC_TIME`|public| |600|

## Properties


### channel_id



```php
protected int $channel_id
```







***

### connections



```php
protected \BigCommerce\Taxonomies\Channel\Connections $connections
```







***

### customers



```php
protected \BigCommerce\Api\v3\Api\CustomersApi $customers
```







***

## Methods


### __construct

Channel_Settings constructor.

```php
public __construct(\BigCommerce\Taxonomies\Channel\Connections $connections, \BigCommerce\Api\v3\Api\CustomersApi $customers): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$connections` | **\BigCommerce\Taxonomies\Channel\Connections** | The Connections instance for managing channels. |
| `$customers` | **\BigCommerce\Api\v3\Api\CustomersApi** | The Customers API instance for updating customer settings. |





***

### get_channel_id

Get the current channel ID.

```php
protected get_channel_id(): int
```

Retrieves the channel ID associated with the current active channel from the Connections instance.







**Return Value:**

The channel ID, or 0 if no channel is found.




***

### sync_global_logins

Sync global logins for the current channel.

```php
public sync_global_logins(): void
```

Updates the global login setting for the current channel. If the channel ID is unavailable,
it will schedule a resync for later.










***

### schedule_resync

Schedule a resync for global logins.

```php
protected schedule_resync(): void
```

Schedules a resync of global logins by setting a single event to trigger
after a predefined interval (RESYNC_TIME).










***

### schedule_sync

Schedule a sync for the channel.

```php
public schedule_sync(): void
```

Triggers a sync for global logins by turning on the option for new channels,
avoiding triggering the update_option listener, and scheduling the sync.










***

### clear_all_scheduled_events

Clear all scheduled events for syncing global logins.

```php
protected clear_all_scheduled_events(): void
```

Clears the scheduled events for the "bigcommerce/sync_global_logins" hook.










***


***
> Automatically generated on 2025-01-07
