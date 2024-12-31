***

# Channel





* Full name: `\BigCommerce\Taxonomies\Channel\Channel`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;bigcommerce_channel&#039;|
|`CHANNEL_ID`|public| |&#039;bigcommerce_channel_id&#039;|
|`STATUS`|public| |&#039;bigcommerce_channel_status&#039;|
|`STATUS_PRIMARY`|public| |&#039;primary&#039;|
|`STATUS_CONNECTED`|public| |&#039;connected&#039;|
|`STATUS_DISCONNECTED`|public| |&#039;disconnected&#039;|
|`STATUS_ORPHAN`|public| |&#039;orphan&#039;|


## Methods


### multichannel_enabled

Get the site's multi-channel support status

```php
public static multichannel_enabled(): bool
```



* This method is **static**.








***

### multichannel_sync_to_all_channels

Should product sync be to all channels?

```php
public static multichannel_sync_to_all_channels(): bool
```



* This method is **static**.








***

### find_by_id



```php
public static find_by_id(int $channel_id): \WP_Term
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$channel_id` | **int** |  |





***

### is_msf_channel_prop_on



```php
public static is_msf_channel_prop_on(string $prop): bool
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$prop` | **string** |  |





***


***
> Automatically generated on 2024-12-31
