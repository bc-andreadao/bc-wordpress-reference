***

# Countries

Class Countries

Handles loading and retrieving country data from a JSON file, and injecting
country data into JavaScript configuration arrays.

* Full name: `\BigCommerce\Accounts\Countries`



## Properties


### data_file



```php
private $data_file
```






***

### data



```php
private $data
```






***

## Methods


### __construct

Countries constructor.

```php
public __construct(string $data_file): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data_file` | **string** | The path to the JSON file containing country data. |





***

### get_countries

Get a list of countries.

```php
public get_countries(): array
```

Loads the country data from the JSON file if it hasn't been loaded yet,
and returns the data as an array.







**Return Value:**

The list of countries loaded from the JSON file.




***

### load_data

Load country data from the JSON file.

```php
private load_data(): void
```

If the country data hasn't already been loaded, this method loads it from the specified
JSON file and decodes it into an array.










***

### js_config

Inject country data into JavaScript configuration.

```php
public js_config(array $config): array
```

Adds the list of countries to the provided JavaScript configuration array under the "countries" key.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$config` | **array** | The JavaScript configuration array to modify. |


**Return Value:**

The modified JavaScript configuration array.




***


***
> Automatically generated on 2024-12-10
