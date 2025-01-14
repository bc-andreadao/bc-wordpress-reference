***

# Customer_Group_Proxy

Class Customer_Group_Proxy

Adds a caching proxy in front of requests for customer group information.

* Full name: `\BigCommerce\Accounts\Customer_Group_Proxy`




## Methods


### filter_group_info

Filter and merge additional customer group info.

```php
public filter_group_info(array $info, int $id): array
```

This method checks if the customer group information is available in the cache;
if not, it fetches it from the API and caches it. The result is merged with the existing
group information before being returned.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$info` | **array** | The existing customer group information. |
| `$id` | **int** | The ID of the customer group. |


**Return Value:**

The merged customer group information.




***


***
> Automatically generated on 2025-01-14
