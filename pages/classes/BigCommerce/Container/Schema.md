***

# Schema

Manages the registration of database schema-related services and roles.

This container handles:
- Database table schema for reviews and queues.
- User roles, including custom roles like "Customer."
- WordPress hooks for table registration and role initialization.

* Full name: `\BigCommerce\Container\Schema`
* Parent class: [`Provider`](./Provider.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`TABLE_REVIEWS`|public|string|&#039;schema.table.reviews&#039;|
|`TABLE_QUEUES`|public|string|&#039;schema.table.queue&#039;|
|`ROLE_SCHEMA`|public|string|&#039;schema.roles&#039;|
|`CUSTOMER_ROLE`|public|string|&#039;schema.roles.customer&#039;|


## Methods


### register

Registers database schema and roles into the container.

```php
public register(\Pimple\Container $container): mixed
```

Services registered:
- Reviews Table schema.
- Queue Table schema.
- Customer Role.
- User Roles schema.

Hooks registered:
- `plugins_loaded`: Registers database tables.
- `admin_init`: Registers user roles.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The DI container for registering services. |





***

### tables

Registers database table-related services and hooks.

```php
private tables(\Pimple\Container $container): mixed
```

Services registered:
- `TABLE_REVIEWS`: Handles the schema for the reviews table.
- `TABLE_QUEUES`: Handles the schema for the queue table.

Hooks registered:
- `plugins_loaded`: Triggers table schema registration.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The DI container for registering services. |





***

### roles

Registers user role-related services and hooks.

```php
private roles(\Pimple\Container $container): mixed
```

Services registered:
- `CUSTOMER_ROLE`: Handles the "Customer" user role.
- `ROLE_SCHEMA`: Manages user roles and their permissions.

Hooks registered:
- `admin_init`: Triggers user role registration.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$container` | **\Pimple\Container** | The DI container for registering services. |





***


***
> Automatically generated on 2024-12-10
