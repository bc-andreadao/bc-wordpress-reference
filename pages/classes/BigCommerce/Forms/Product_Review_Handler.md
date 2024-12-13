***

# Product_Review_Handler





* Full name: `\BigCommerce\Forms\Product_Review_Handler`
* This class implements:
[`\BigCommerce\Forms\Form_Handler`](./classes/BigCommerce/Forms/Form_Handler.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;product-review&#039;|


## Methods


### __construct

Product_Review_Handler constructor.

```php
public __construct(\BigCommerce\Api\v3\Api\CatalogApi $api): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$api` | **\BigCommerce\Api\v3\Api\CatalogApi** | The API instance to interact with BigCommerce&#039;s catalog. |





***

### handle_request

Handle the form submission for product reviews.

```php
public handle_request(array $submission): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **array** | The form submission data. |





***

### remove_form_messages_from_post_content

Do not show product review form error/success messages above
the post content. They will be rendered with the form.

```php
public remove_form_messages_from_post_content(bool $show, int $post_id): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$show` | **bool** | Whether to show messages above content. |
| `$post_id` | **int** | The post ID to check. |


**Return Value:**

Whether to show the messages.




***

### toggle_reviews_form_availability

Handle the visibility of the product reviews form.

```php
public toggle_reviews_form_availability(bool $enabled, int $post_id): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$enabled` | **bool** | Whether the form is enabled. |
| `$post_id` | **int** | The post ID to check. |


**Return Value:**

Whether to display the reviews form.




***


***
> Automatically generated on 2024-12-13
