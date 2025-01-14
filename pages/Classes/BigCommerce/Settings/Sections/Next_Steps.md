***

# Next_Steps

Class Next_Steps

Displays required and optional next steps after onboarding.

* Full name: `\BigCommerce\Settings\Sections\Next_Steps`
* Parent class: [`\BigCommerce\Settings\Sections\Settings_Section`](./classes/BigCommerce/Settings/Sections/Settings_Section.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public| |&#039;next_steps&#039;|


## Methods


### __construct



```php
public __construct(\BigCommerce\Merchant\Setup_Status $status, mixed $template_dir): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$status` | **\BigCommerce\Merchant\Setup_Status** |  |
| `$template_dir` | **mixed** |  |





***

### register_settings_section



```php
public register_settings_section(): mixed
```












***

### render_section



```php
public render_section(): mixed
```












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
> Automatically generated on 2025-01-14
