***

# Task_Manager

Class Task_Manager

Responsible for coordinating the sequence of import tasks

* Full name: `\BigCommerce\Import\Task_Manager`




## Methods


### register

Register a new task

```php
public register(\BigCommerce\Import\Task_Definition $task): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$task` | **\BigCommerce\Import\Task_Definition** |  |





***

### unregister

Remove a task from the registry

```php
public unregister(\BigCommerce\Import\Task_Definition $task): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$task` | **\BigCommerce\Import\Task_Definition** |  |





***

### get_task



```php
public get_task(string $state): \BigCommerce\Import\Task_Definition
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$state` | **string** | The current state of the import |





***

### run_next

Run the next task in the queue

```php
public run_next(string $state): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$state` | **string** |  |





***

### task_count

Get the total count of registered tasks

```php
public task_count(): int
```












***

### completed_count

Get the count of tasks completed to get to the current state

```php
public completed_count(mixed $state): int
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$state` | **mixed** |  |




**Throws:**

- [`No_Task_Found_Exception`](./classes/BigCommerce/Exceptions/No_Task_Found_Exception.md)



***


***
> Automatically generated on 2025-01-14
