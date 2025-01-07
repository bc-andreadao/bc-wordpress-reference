***

# Customer

Class Customer

A user role with no capabilities, not even `read`. This class represents a "Customer" role
in the BigCommerce accounts system. It implements the `Role` interface and provides
methods to retrieve the role's ID and label.

* Full name: `\BigCommerce\Accounts\Roles\Customer`
* This class implements:
[`\BigCommerce\Accounts\Roles\Role`](./classes/BigCommerce/Accounts/Roles/Role.md)


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`NAME`|public|string|&#039;customer&#039;|


## Methods


### get_id

Gets the ID of the customer role.

```php
public get_id(): string
```

This method returns the unique identifier for the `Customer` role, which is the
value of the `NAME` constant (`'customer'`).







**Return Value:**

The ID of the customer role.




***

### get_label

Gets the label of the customer role.

```php
public get_label(): string
```

This method returns the label for the `Customer` role, which is a translatable string.
It is typically used to display the role's name in a UI.







**Return Value:**

The label of the customer role.




***


***
> Automatically generated on 2025-01-07
