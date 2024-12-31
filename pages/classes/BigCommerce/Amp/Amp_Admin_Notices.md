***

# Amp_Admin_Notices

Creates an admin notice if requirements for AMP + BC or not met.

Handles the display of admin notices related to AMP and BigCommerce integration.
Specifically, it checks if AMP is active and whether the site is using SSL,
displaying relevant notices in the WordPress admin interface.

* Full name: `\BigCommerce\Amp\Amp_Admin_Notices`




## Methods


### __construct

Constructor

```php
public __construct(string $screen_id, bool $amp_is_enabled = false, bool $is_ssl = null): mixed
```

Initializes the Amp_Admin_Notices object with necessary information
including the screen ID, AMP plugin status, and SSL status.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$screen_id` | **string** | ID of the admin screen where the notice will appear. |
| `$amp_is_enabled` | **bool** | Whether the AMP plugin is active. Default is false. |
| `$is_ssl` | **bool** | Whether the site uses SSL. Default is null, which checks the current SSL status. |





***

### get_notices

Provides the instance's notices.

```php
public get_notices(): array
```









**Return Value:**

List of notices to be displayed.




***

### add_notice

Adds a notice to the instance's notices list.

```php
public add_notice(string $notice): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$notice` | **string** | The notice message to be added. |





***

### render_amp_admin_notices

Displays an admin notice if AMP is active and SSL is not enabled.

```php
public render_amp_admin_notices(): mixed
```

This method renders the AMP-related admin notices in the WordPress dashboard.
It checks whether AMP is active, whether the current screen matches the provided
screen ID, and whether the SSL notice should be displayed.










***


***
> Automatically generated on 2024-12-31
