***

# Build_Docs

Register build docs command and related functionality



* Full name: `\BigCommerce\CLI\Documentation\Build_Docs`
* Parent class: [`\BigCommerce\CLI\Command`](./classes/BigCommerce/CLI/Command.md)




## Methods


### __construct

Constructor for the Build_Docs class.

```php
public __construct(string $plugin_dir): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$plugin_dir` | **string** | Directory path of the plugin. |





***

### command

Declare command name.

```php
protected command(): string
```









**Return Value:**

The CLI command name.




***

### description

Provide a command description.

```php
protected description(): string|void
```









**Return Value:**

The CLI command description.




***

### arguments

Declare command arguments.

```php
protected arguments(): array[]
```









**Return Value:**

List of command arguments.




***

### run

Get files data and write it to the provided file.

```php
public run(array $args, array $assoc_args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | Positional arguments passed to the command. |
| `$assoc_args` | **array** | Associative arguments passed to the command. |




**Throws:**
<p>If there is an issue during execution.</p>

- [`ExitException`](./classes/WP_CLI/ExitException.md)



***


## Inherited methods


### register

Register the command with WP-CLI.

```php
public register(): void
```

This method checks if WP-CLI is defined and active. If so, it registers the command
with WP-CLI, using the specific command name defined in the child class.










***

### command

Get the command name.

```php
protected command(): string
```

This method must be implemented in the child class to return the specific command name.


* This method is **abstract**.




**Return Value:**

The name of the WP-CLI command.




***

### description

Get a short description of the command.

```php
protected description(): string
```

This method must be implemented in the child class to provide a brief description
of the command's functionality, which will be shown in the WP-CLI help output.


* This method is **abstract**.




**Return Value:**

The short description of the command.




***

### arguments

Get the command arguments.

```php
protected arguments(): string
```

This method must be implemented in the child class to return the arguments
required by the command. The arguments will be shown in the WP-CLI help output.


* This method is **abstract**.




**Return Value:**

The arguments for the command.




***

### run

Run the command.

```php
public run(array $args, array $assoc_args): void
```

This method must be implemented in the child class to define the logic
for executing the command. It accepts arguments and associative arguments
passed to the command via WP-CLI.


* This method is **abstract**.



**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | The positional arguments passed to the command. |
| `$assoc_args` | **array** | The associative arguments passed to the command. |





***


***
> Automatically generated on 2025-01-13
