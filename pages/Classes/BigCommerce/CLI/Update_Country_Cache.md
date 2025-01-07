***

# Update_Country_Cache

Updates the country and state cache in a JSON file located at assets/data/countries.json.

This command fetches the latest country and state data from the BigCommerce API and stores it in a specified output file.
If no output file is provided, it defaults to a predefined file path.

Usage: wp bigcommerce countries update --output=/path/to/file.json

* Full name: `\BigCommerce\CLI\Update_Country_Cache`
* Parent class: [`\BigCommerce\CLI\Command`](./classes/BigCommerce/CLI/Command.md)




## Methods


### __construct

Constructor to initialize the default output file.

```php
public __construct(string $default_output_file): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$default_output_file` | **string** | The default file path for the JSON output. |





***

### command

Declare the WP-CLI command for updating the country cache.

```php
protected command(): string
```









**Return Value:**

The WP-CLI command to execute.




***

### description

Add a description for the WP-CLI command.

```php
protected description(): string
```









**Return Value:**

The description of the command.




***

### arguments

Declare the command arguments for the update cache operation.

```php
protected arguments(): array[]
```









**Return Value:**

The command arguments, including an optional output file argument.




***

### run

Executes the update process for the country and state cache.

```php
public run(array $args, array $assoc_args): void
```

Fetches data from the BigCommerce API and writes it to the specified output file.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | Arguments passed to the command. |
| `$assoc_args` | **array** | Associated arguments (e.g., output file path). |




**Throws:**
<p>If there is an error in the process, an exit exception is thrown.</p>

- [`ExitException`](./classes/WP_CLI/ExitException.md)



***

### get_country_data

Fetches the country and state data from the BigCommerce API.

```php
public get_country_data(): array
```

Retrieves a list of countries and their respective states, if available.







**Return Value:**

An array of countries with associated state data.




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
