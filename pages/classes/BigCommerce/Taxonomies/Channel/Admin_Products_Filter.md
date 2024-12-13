***

# Admin_Products_Filter

Class Admin_Products_Filter

Responsible for filtering the products in the admin list table by channel ID

* Full name: `\BigCommerce\Taxonomies\Channel\Admin_Products_Filter`




## Methods


### display_channel_select

Display the channel select above the Products list table

```php
public display_channel_select(string $post_type, string $which): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_type` | **string** |  |
| `$which` | **string** |  |





***

### filter_list_table_request

Enforce a channel filter when displaying the products list table
by setting query vars on the request

```php
public filter_list_table_request(\WP $request): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$request` | **\WP** |  |





***


***
> Automatically generated on 2024-12-13
