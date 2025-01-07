***

# Welcome_Screen

Abstract base class for managing plugin settings screens.

This abstract class provides a foundation for settings screens in the WordPress admin.
It defines common properties such as the hook suffix, capability, and asset URL,
along with the constant `NAME` which should be defined in concrete subclasses.
Concrete subclasses should implement their specific logic for rendering the screen
and handling settings.

* Full name: `\BigCommerce\Settings\Screens\Welcome_Screen`
* Parent class: [`\BigCommerce\Settings\Screens\Onboarding_Screen`](./classes/BigCommerce/Settings/Screens/Onboarding_Screen.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;bigcommerce_welcome&#039;|


## Methods


### __construct

Abstract_Screen constructor.

```php
public __construct(mixed $configuration_status, mixed $assets_url, mixed $template_dir): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$configuration_status` | **mixed** | A flag indicating if the current stage in the setup process. |
| `$assets_url` | **mixed** | Path to the plugin assets directory. |
| `$template_dir` | **mixed** |  |





***

### get_page_title

Gets the title to render for the page.

```php
protected get_page_title(): string
```









**Return Value:**

The title to render for the page.




***

### get_menu_title

Gets the title to show in the admin menu for the page.

```php
protected get_menu_title(): string
```









**Return Value:**

The title to show in the admin menu for the page.




***

### render_settings_page

Renders the settings page.

```php
public render_settings_page(): void
```












***

### should_register

Indicates if this screen should be registered, given the current state of the WordPress installation.

```php
public should_register(): bool
```









**Return Value:**

True if the screen should be registered, false otherwise.




***


## Inherited methods


### __construct

Abstract_Screen constructor.

```php
public __construct(int $configuration_status, string $assets_url): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$configuration_status` | **int** | A flag indicating if the current stage in the setup process. |
| `$assets_url` | **string** | Path to the plugin assets directory. |





***

### get_page_title

Gets the title to render for the page.

```php
protected get_page_title(): string
```




* This method is **abstract**.




**Return Value:**

The title to render for the page.




***

### get_menu_title

Gets the title to show in the admin menu for the page.

```php
protected get_menu_title(): string
```




* This method is **abstract**.




**Return Value:**

The title to show in the admin menu for the page.




***

### get_header

Retrieves the header HTML for the settings page.

```php
protected get_header(): string
```

This method generates the header for the settings page, including the page title wrapped
in an `<h1>` tag. If the title is empty, it returns an empty string.

The title is obtained by calling the `get_page_title()` method, and additional content
may be prepended to the title using the `before_title()` method.







**Return Value:**

The HTML markup for the header, or an empty string if no title is provided.




***

### before_title

Generates the markup before the page title.

```php
protected before_title(): string
```

This method outputs a placeholder to indicate where notices should be placed
within the WordPress admin header. It also fires the `bigcommerce/settings/before_title/page={NAME}`
action hook, allowing other components to hook into this point and potentially add additional content.







**Return Value:**

The HTML markup for the section before the title.




***

### get_hook_suffix

Gets the hook suffix for the settings page.

```php
public get_hook_suffix(): string
```









**Return Value:**

The hook suffix for the settings page.




***

### get_url

Gets the URL for the settings page.

```php
public get_url(): string
```









**Return Value:**

The URL for the settings page.




***

### register_settings_page

Registers the settings page in the WordPress admin menu.

```php
public register_settings_page(): void
```












***

### get_capability

Gets the capability required to view the settings page.

```php
public get_capability(): string
```









**Return Value:**

The capability required to view the settings page.




***

### parent_slug

Retrieves the parent slug for the settings page.

```php
protected parent_slug(): string
```

This method generates the parent URL slug for the settings page by formatting the URL
with the post type constant from the `Product` class.







**Return Value:**

The formatted parent slug for the settings page.




***

### render_settings_page

Renders the settings page.

```php
public render_settings_page(): void
```












***

### progress_bar

Renders the onboarding progress bar for the current screen.

```php
protected progress_bar(): string
```









**Return Value:**

The HTML markup for the progress bar.




***

### start_form

Starts the form for the settings page.

```php
protected start_form(): void
```












***

### end_form

Ends the form for the settings page.

```php
protected end_form(): void
```












***

### form_action_url

Gets the URL to which the form will submit.

```php
protected form_action_url(): string
```









**Return Value:**

The form action URL.




***

### settings_fields

Renders the hidden settings fields for the form.

```php
protected settings_fields(): void
```












***

### submit_button

Renders the submit button for the settings form.

```php
protected submit_button(): void
```












***

### before_form

Renders content before the settings form starts.

```php
protected before_form(): void
```












***

### after_form

Renders content after the settings form finishes.

```php
protected after_form(): void
```












***

### do_settings_sections

Renders the settings sections for the settings page.

```php
protected do_settings_sections(string $page): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$page` | **string** | The settings page. |





***

### section_header

Renders the header for the settings section.

```php
protected section_header(array $section, string $page): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$section` | **array** | The settings section. |
| `$page` | **string** | The settings page. |





***

### section_body

Renders the body for the settings section.

```php
protected section_body(array $section, string $page): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$section` | **array** | The settings section. |
| `$page` | **string** | The settings page. |





***

### setup_unregistered_redirect

Sets up a redirect for unregistered screens in the admin menu.

```php
protected setup_unregistered_redirect(): void
```

This method ensures that if the current screen is not registered,
a redirection is set up to trigger the `bigcommerce/settings/unregistered_screen` action.
It is only called if the global `plugin_page` matches the screen's NAME constant.










***

### redirect_to_screen

Redirects to the current settings screen.

```php
public redirect_to_screen(): void
```












***

### should_register

Indicates if this screen should be registered, given the current state of the WordPress installation.

```php
public should_register(): bool
```









**Return Value:**

True if the screen should be registered, false otherwise.




***

### set_admin_body_class

Sets the body class for the admin page.

```php
public set_admin_body_class(string $classes = &#039;&#039;): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$classes` | **string** | The existing body classes. |


**Return Value:**

The modified body classes.




***

### get_admin_body_class

Gets the class for the admin body.

```php
protected get_admin_body_class(): string
```









**Return Value:**

The admin body class.




***

### onboarding_page_header



```php
protected onboarding_page_header(): mixed
```












***

### onboarding_submit_button



```php
protected onboarding_submit_button(mixed $data_attr_name, mixed $classes, mixed $button_label, mixed $hide_label = false): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data_attr_name` | **mixed** |  |
| `$classes` | **mixed** |  |
| `$button_label` | **mixed** |  |
| `$hide_label` | **mixed** |  |





***

### make_video_embed



```php
protected make_video_embed(mixed $url, mixed $width = 1280, mixed $height = 720): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$url` | **mixed** |  |
| `$width` | **mixed** |  |
| `$height` | **mixed** |  |





***


***
> Automatically generated on 2025-01-07
