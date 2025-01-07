***

# Reset_Plugin

Resets various options in WordPress to bring the site back to the beginning of the BigCommerce account onboarding flow.

This command deletes key options related to the BigCommerce integration, allowing the user to restart the onboarding process.

Usage: wp bigcommerce dev reset-plugin

* Full name: `\BigCommerce\CLI\Reset_Plugin`
* Parent class: [`\BigCommerce\CLI\Command`](./classes/BigCommerce/CLI/Command.md)




## Methods


### command

Declare the command name.

```php
protected command(): string
```









**Return Value:**

The command name for resetting the plugin.




***

### description

Add a command description.

```php
protected description(): string|void
```









**Return Value:**

A description of the reset-plugin command.




***

### arguments

Declare command arguments.

```php
protected arguments(): array[]
```









**Return Value:**

Command arguments for the reset-plugin command.




***

### run

Executes the reset process by deleting specific options from the database.

```php
public run(array $args, array $assoc_args): void
```

This method deletes a set of options that are related to the BigCommerce integration, effectively resetting the state of the plugin
so that the user can restart the onboarding process.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | Arguments passed to the command. |
| `$assoc_args` | **array** | Associated arguments. |





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
> Automatically generated on 2025-01-07
