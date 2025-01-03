***

# Customer_Group

Class Customer_Group

Represents a customer group in BigCommerce and provides methods to retrieve group information.

* Full name: `\BigCommerce\Accounts\Customer_Group`




## Methods


### __construct

Customer_Group constructor.

```php
public __construct(int $group_id): mixed
```

Initializes the customer group with the specified group ID.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$group_id` | **int** | The ID of the customer group. |





***

### get_info

Get information about the customer group.

```php
public get_info(): array
```

Retrieves information about the customer group, including:
- id             (int)    The group ID
- name           (string) The group name
- is_default     (bool)   Whether the group is the default for new customers
- discount_rules (array)  Discount rules applied to the group

The returned data can be filtered using the `bigcommerce/customer/group_info` filter.







**Return Value:**

The customer group information.




***


***
> Automatically generated on 2025-01-03
