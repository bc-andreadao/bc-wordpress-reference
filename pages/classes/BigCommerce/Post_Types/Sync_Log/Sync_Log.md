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

## Properties


### sync_id



```php
private $sync_id
```






***

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

### get_post_date_formatted

Get formatted post date

```php
private get_post_date_formatted(\WP_Post $post): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post` | **\WP_Post** |  |





***

### get_timezone_string

Get the timezone string

```php
private get_timezone_string(): string
```












***

### get_current_sync_id

Get the sync ID

```php
private get_current_sync_id(): int
```












***

### remove_old_syncs

Remove old sync logs

```php
private remove_old_syncs(mixed $status = &#039;draft&#039;, mixed $keep): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$status` | **mixed** |  |
| `$keep` | **mixed** |  |





***

### get_summary_formatted

Get formatted summary

```php
private get_summary_formatted(\WP_Post $sync_log): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$sync_log` | **\WP_Post** |  |





***

### get_multichannel_summary_formatted

Get formatted summary

```php
private get_multichannel_summary_formatted(\WP_Post $sync_log): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$sync_log` | **\WP_Post** |  |





***


***
> Automatically generated on 2024-12-10
