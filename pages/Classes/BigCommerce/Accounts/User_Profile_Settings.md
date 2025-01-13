***

# User_Profile_Settings

Class User_Profile_Settings

Responsible for rendering and saving user profile settings, specifically for synchronizing passwords
between WordPress and the BigCommerce API.

* Full name: `\BigCommerce\Accounts\User_Profile_Settings`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`SYNC_PASSWORD`|public| |&#039;bigcommerce_sync_password&#039;|
|`NONCE_ACTION`|public| |&#039;bc_user_profile&#039;|
|`NONCE_NAME`|public| |&#039;bc_nonce&#039;|


## Methods


### render_profile_settings

Render profile settings

```php
public render_profile_settings(\WP_User $user): void
```

This action is triggered on the user profile page to display BigCommerce-specific settings, such as
synchronizing passwords with the BigCommerce API.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$user` | **\WP_User** | The user object for which the settings are being rendered. |





***

### save_profile_settings

Handle save logic for profile settings

```php
public save_profile_settings(int $user_id): void
```

This action is triggered when the user profile settings are saved, allowing for synchronization
of passwords between WordPress and the BigCommerce API.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$user_id` | **int** | The ID of the user whose settings are being saved. |





***


***
> Automatically generated on 2025-01-13
