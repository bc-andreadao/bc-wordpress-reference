***

# Role

Interface Role

An interface for defining user roles in the BigCommerce accounts system. Any role class
that implements this interface must provide methods to retrieve the role's unique identifier
and its label.

* Full name: `\BigCommerce\Accounts\Roles\Role`



## Methods


### get_id

Gets the ID of the role.

```php
public get_id(): string
```

This method must be implemented by any class that represents a user role. It should
return a unique identifier for the role, typically a string constant or similar value.







**Return Value:**

The ID of the role.




***

### get_label

Gets the label of the role.

```php
public get_label(): string
```

This method must be implemented by any class that represents a user role. It should
return a translatable label or name for the role, typically used for display purposes
in the user interface.







**Return Value:**

The label of the role.




***


***
> Automatically generated on 2024-12-13
