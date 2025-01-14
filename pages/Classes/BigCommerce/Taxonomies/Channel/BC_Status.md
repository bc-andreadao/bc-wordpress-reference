***

# BC_Status





* Full name: `\BigCommerce\Taxonomies\Channel\BC_Status`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`STATUS`|public| |&#039;bigcommerce_channel_bc_status&#039;|
|`STATUS_ACTIVE`|public| |&#039;active&#039;|
|`STATUS_INACTIVE`|public| |&#039;inactive&#039;|
|`STATUS_DELETED`|public| |&#039;deleted&#039;|
|`STATUS_ARCHIVED`|public| |&#039;archived&#039;|
|`STATUS_PRE_LAUNCH`|public| |&#039;prelaunch&#039;|


## Methods


### maybe_cancel_import

Prevent product import for non active status

```php
public maybe_cancel_import(): void
```












***

### admin_notices

Show admin notices for non active status

```php
public admin_notices(): void
```












***

### get_current_channel_status

Get current channel status

```php
public get_current_channel_status(): string
```












***


***
> Automatically generated on 2025-01-14
