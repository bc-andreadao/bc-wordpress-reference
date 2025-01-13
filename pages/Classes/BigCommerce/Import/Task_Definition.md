***

# Task_Definition





* Full name: `\BigCommerce\Import\Task_Definition`




## Methods


### __construct

Task_Definition constructor.

```php
public __construct(callable $callback, int $priority, string $completion_state, array $in_progress_states = [], string $description = &#039;&#039;): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$callback` | **callable** | The callback to run this task |
| `$priority` | **int** | The order in which the task should run. Lower values run before higher values. |
| `$completion_state` | **string** | The state at which this task is considered complete |
| `$in_progress_states` | **array** | An array of optional interim states where the task should keep running. |
| `$description` | **string** | A user-friendly description of the task |





***

### get_callback



```php
public get_callback(): mixed
```












***

### get_priority



```php
public get_priority(): mixed
```












***

### get_completion_state



```php
public get_completion_state(): mixed
```












***

### get_in_progress_states



```php
public get_in_progress_states(): mixed
```












***

### get_description



```php
public get_description(): mixed
```












***


***
> Automatically generated on 2025-01-13
