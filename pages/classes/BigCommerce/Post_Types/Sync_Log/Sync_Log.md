***

# Sync_Log





* Full name: `\BigCommerce\Post_Types\Sync_Log\Sync_Log`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;bigcommerce_sync_log&#039;|
|`META_STATUS`|public| |&#039;status&#039;|
|`META_EVENT`|public| |&#039;event&#039;|
|`META_ERRORS`|public| |&#039;errors&#039;|
|`META_SUMMARY`|public| |&#039;summary&#039;|
|`META_DURATION`|public| |&#039;duration&#039;|
|`MULTICHANNEL_SUMMARY`|public| |&#039;multichannel_summary&#039;|
|`MULTICHANNEL_ACTIVE`|public| |&#039;multichannel_active&#039;|


## Methods


### create_sync

Create a draft sync log

```php
public create_sync(): void
```












***

### complete_sync

Called on import complete

```php
public complete_sync(array $log): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$log` | **array** | The current log |





***

### log_error

Store errors

```php
public log_error(mixed $error): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$error` | **mixed** |  |





***

### diagnostic_data

Add sync logs to Diagnostics panel

```php
public diagnostic_data(array $data): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **array** |  |





***


***
> Automatically generated on 2024-12-10
