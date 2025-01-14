***

# Command

This is an abstract base class for creating custom WP-CLI commands in the BigCommerce CLI namespace.

It registers the command with WP-CLI and provides methods for handling command-specific logic.

* Full name: `\BigCommerce\CLI\Command`
* Parent class: [`WP_CLI_Command`](./classes/WP_CLI_Command.md)
* This class is an **Abstract class**




## Methods


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
