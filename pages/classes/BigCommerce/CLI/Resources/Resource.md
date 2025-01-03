***

# Resource

Class Resource

Represents a resource with various properties such as URL, name, description, thumbnails, categories, and external status.
Implements the JsonSerializable interface to allow conversion to JSON.

* Full name: `\BigCommerce\CLI\Resources\Resource`
* This class implements:
[`\JsonSerializable`](./classes/JsonSerializable.md)




## Methods


### get_url

Get the URL of the resource.

```php
public get_url(): string
```









**Return Value:**

The URL of the resource.




***

### set_url

Set the URL of the resource.

```php
public set_url(string $url): resource
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$url` | **string** | The URL of the resource. |


**Return Value:**

The current instance of the resource.




***

### get_name

Get the name of the resource.

```php
public get_name(): string
```









**Return Value:**

The name of the resource.




***

### set_name

Set the name of the resource.

```php
public set_name(string $name): resource
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$name` | **string** | The name of the resource. |


**Return Value:**

The current instance of the resource.




***

### get_description

Get the description of the resource.

```php
public get_description(): string
```









**Return Value:**

The description of the resource.




***

### set_description

Set the description of the resource.

```php
public set_description(string $description): resource
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$description` | **string** | The description of the resource. |


**Return Value:**

The current instance of the resource.




***

### get_thumbnail

Get the thumbnail URL of the resource.

```php
public get_thumbnail(): string
```









**Return Value:**

The thumbnail URL of the resource.




***

### set_thumbnail

Set the thumbnail URL of the resource.

```php
public set_thumbnail(string $thumbnail): resource
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$thumbnail` | **string** | The thumbnail URL of the resource. |


**Return Value:**

The current instance of the resource.




***

### get_hires_thumbnail

Get the high-resolution thumbnail URL of the resource.

```php
public get_hires_thumbnail(): string
```









**Return Value:**

The high-resolution thumbnail URL of the resource.




***

### set_hires_thumbnail

Set the high-resolution thumbnail URL of the resource.

```php
public set_hires_thumbnail(string $hires_thumbnail): resource
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$hires_thumbnail` | **string** | The high-resolution thumbnail URL of the resource. |


**Return Value:**

The current instance of the resource.




***

### get_external

Get the external status of the resource.

```php
public get_external(): bool
```









**Return Value:**

Whether the resource is external or not.




***

### set_external

Set the external status of the resource.

```php
public set_external(bool $external): resource
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$external` | **bool** | Whether the resource is external or not. |


**Return Value:**

The current instance of the resource.




***

### get_categories

Get the categories associated with the resource.

```php
public get_categories(): string[]
```









**Return Value:**

The list of categories associated with the resource.




***

### set_categories

Set the categories associated with the resource.

```php
public set_categories(string[] $categories): resource
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$categories` | **string[]** | The list of categories to associate with the resource. |


**Return Value:**

The current instance of the resource.




***

### jsonSerialize

Specify data to be serialized to JSON.

```php
public jsonSerialize(): array
```









**Return Value:**

Data representing the object for JSON encoding.




***


***
> Automatically generated on 2025-01-03
