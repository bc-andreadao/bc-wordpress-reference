***

# Channels

Class Channels

Channel configuration after the plugin has been fully configured,
which at this point is limited to changing the channel name

* Full name: `\BigCommerce\Settings\Sections\Channels`
* Parent class: [`\BigCommerce\Settings\Sections\Settings_Section`](./classes/BigCommerce/Settings/Sections/Settings_Section.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;channel&#039;|
|`CHANNEL_ID`|public| |&#039;bigcommerce_channel_id&#039;|
|`CHANNEL_NAME`|public| |&#039;bigcommerce_channel_name&#039;|
|`NEW_NAME`|public| |&#039;bigcommerce_add_channel_name&#039;|
|`PRIMARY_CHANNEL`|public| |&#039;bigcommerce_primary_channel&#039;|
|`CONNECTED_CHANNELS`|public| |&#039;bigcommerce_connected_channels&#039;|
|`OTHER_CHANNELS`|public| |&#039;bigcommerce_other_channels&#039;|
|`ACTION_RENAME`|public| |&#039;rename&#039;|
|`ACTION_CONNECT`|public| |&#039;connect&#039;|
|`ACTION_DISCONNECT`|public| |&#039;disconnect&#039;|
|`ACTION_PROMOTE`|public| |&#039;promote&#039;|
|`POST_ACTION`|public| |&#039;bigcommerce-channel-operation&#039;|


## Methods


### register_settings_section



```php
public register_settings_section(): mixed
```












***

### render_primary_channel



```php
public render_primary_channel(): mixed
```












***

### render_connected_channels



```php
public render_connected_channels(): mixed
```












***

### render_other_channels



```php
public render_other_channels(): mixed
```












***

### handle_action_submission

Handle a request to perform an operation on an existing channel

```php
public handle_action_submission(string $redirect): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$redirect` | **string** | URL to redirect to after handling the submission |





***

### promote_channel

Promote a channel to the "Primary" status, demoting
the current primary to the "Connected" status

```php
public promote_channel(\WP_Term $term): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$term` | **\WP_Term** |  |





***

### save_channel_names

Save channel name changes to taxonomy terms, not to options

```php
public save_channel_names(array $value): null
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **array** |  |





***


## Inherited methods


### render_field



```php
public render_field(array $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** |  |





***

### render_number_field



```php
public render_number_field(array $args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** |  |





***

### get_disabled_attr_headless

Get disabled attribute if headless option is on

```php
public get_disabled_attr_headless(): string
```












***


***
> Automatically generated on 2024-12-31
