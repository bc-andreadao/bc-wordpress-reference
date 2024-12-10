***

# Deletion





* Full name: `\BigCommerce\Post_Types\Product\Deletion`




## Methods


### delete_product_data



```php
public delete_product_data(int $post_id): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** |  |





***

### remove_images

Remove all images related to the product

```php
private remove_images(int $post_id): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** |  |





***

### reparent_images

Set the attachment parent to a new post

```php
private reparent_images(int $old_parent_id, int $new_parent_id): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$old_parent_id` | **int** |  |
| `$new_parent_id` | **int** |  |





***

### identify_child_attachments

Find all imported attachments with the given post as a parent

```php
private identify_child_attachments(int $post_id): int[]
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** |  |





***

### get_post_in_another_channel

Determine if there are other posts with the same product ID in other channels

```php
private get_post_in_another_channel(int $bc_id, int $post_id): int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$bc_id` | **int** |  |
| `$post_id` | **int** |  |


**Return Value:**

A post ID for the product in another channel




***


***
> Automatically generated on 2024-12-10
