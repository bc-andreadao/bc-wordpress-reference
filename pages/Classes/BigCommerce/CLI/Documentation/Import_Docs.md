***

# Import_Docs

Class Import_Docs

Handles the import of plugin documentation from a previously built JSON file.

* Full name: `\BigCommerce\CLI\Documentation\Import_Docs`
* Parent class: [`\BigCommerce\CLI\Command`](./classes/BigCommerce/CLI/Command.md)




## Methods


### __construct

Import_Docs constructor.

```php
public __construct(string $plugin_dir): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$plugin_dir` | **string** | Directory of the plugin. |





***

### command

Declare the command name.

```php
protected command(): string
```












***

### description

Provide a command description.

```php
protected description(): string
```












***

### arguments

Declare command arguments.

```php
protected arguments(): array[]
```












***

### run

Execute the documentation import process.

```php
public run(array $args, array $assoc_args): void
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | Positional arguments passed to the command. |
| `$assoc_args` | **array** | Associative arguments passed to the command. |




**Throws:**

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
> Automatically generated on 2025-01-14
