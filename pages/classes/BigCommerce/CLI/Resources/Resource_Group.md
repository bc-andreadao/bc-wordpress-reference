***

# Resource_Group

Represents a group of resources, which are categorized by a label.

Implements the JsonSerializable interface to allow conversion to JSON.

* Full name: `\BigCommerce\CLI\Resources\Resource_Group`
* This class implements:
[`\JsonSerializable`](./classes/JsonSerializable.md)




## Methods


### __construct

Resource_Group constructor.

```php
public __construct(string $label): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$label` | **string** | The label for the resource group. |





***

### add_resource

Add a resource to the group.

```php
public add_resource(resource $resource): $this
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$resource` | **resource** | The resource to add to the group. |


**Return Value:**

The current instance of the group.




***

### get_label

Get the label of the resource group.

```php
public get_label(): string
```









**Return Value:**

The label of the group.




***

### get_resources

Get the list of resources in the group.

```php
public get_resources(): resource[]
```









**Return Value:**

The resources within the group.




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
> Automatically generated on 2024-12-13
