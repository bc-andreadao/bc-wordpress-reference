***

# Import_Now





* Full name: `\BigCommerce\Settings\Import_Now`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public| |&#039;bigcommerce_import_now&#039;|


## Methods


### __construct

Import_Now constructor.

```php
public __construct(\BigCommerce\Settings\Screens\Settings_Screen $settings_screen): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$settings_screen` | **\BigCommerce\Settings\Screens\Settings_Screen** |  |





***

### render_button



```php
public render_button(string $label = &#039;&#039;, string $redirect = &#039;&#039;): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$label` | **string** | The label for the button. |
| `$redirect` | **string** | The redirect destination after starting the import. Defaults to the settings page. |





***

### list_table_link

Add the sync link to the views above the products
list table. While not exactly a view, it's a reasonable place
to inject the status into the UI.

```php
public list_table_link(array $views = []): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$views` | **array** |  |





***

### get_import_url



```php
public get_import_url(string $redirect = &#039;&#039;): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$redirect` | **string** |  |





***

### handle_request



```php
public handle_request(): void
```












***

### list_table_notice

Print the import button into the notices section
of the products admin list table.

```php
public list_table_notice(): void
```












***


***
> Automatically generated on 2024-12-13
