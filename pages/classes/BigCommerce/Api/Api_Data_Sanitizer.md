***

# Api_Data_Sanitizer

Trait Api_Data_Sanitizer

Provides methods to sanitize various types of data.

This trait contains helper methods for sanitizing and normalizing different
types of data such as integers, doubles, strings, booleans, and dates. These
methods ensure that the data is properly formatted before being used in the
application.

* Full name: `\BigCommerce\Api\Api_Data_Sanitizer`




## Methods


### sanitize_int

Sanitizes an integer value.

```php
protected sanitize_int(mixed $value): int
```

This method converts a scalar value to an integer. If the value is not
scalar (e.g., an array or object), it returns 0.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** | The value to sanitize. |


**Return Value:**

The sanitized integer value.




***

### sanitize_double

Sanitizes a double (floating-point) value.

```php
protected sanitize_double(mixed $value): float
```

This method converts a scalar value to a double. If the value is not
scalar (e.g., an array or object), it returns 0.0.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** | The value to sanitize. |


**Return Value:**

The sanitized double value.




***

### sanitize_string

Sanitizes a string value.

```php
protected sanitize_string(mixed $value): string
```

This method converts a scalar value to a string. If the value is not
scalar (e.g., an array or object), it returns an empty string.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** | The value to sanitize. |


**Return Value:**

The sanitized string value.




***

### sanitize_bool

Sanitizes a boolean value.

```php
protected sanitize_bool(mixed $value): bool
```

This method converts a scalar value to a boolean. If the value is not
scalar (e.g., an array or object), it returns false.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** | The value to sanitize. |


**Return Value:**

The sanitized boolean value.




***

### sanitize_date

Sanitizes a date value.

```php
protected sanitize_date(mixed $value): string
```

This method formats a `DateTime` object to a string in 'Y-m-d H:i:s' format.
If the value is not a `DateTime` object, it returns the current time in
MySQL format.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$value` | **mixed** | The value to sanitize. |


**Return Value:**

The sanitized date value in 'Y-m-d H:i:s' format.




***

***
> Automatically generated on 2024-12-13

