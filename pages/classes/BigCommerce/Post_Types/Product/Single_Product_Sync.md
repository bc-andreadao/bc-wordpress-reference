***

# Single_Product_Sync

Class Single_Product_Sync

Adds a link to the post actions row to sync a single product with BigCommerce.

* Full name: `\BigCommerce\Post_Types\Product\Single_Product_Sync`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;sync-product&#039;|


## Methods


### add_row_action

Adds the "Re-sync" action to the product post row actions in the admin panel.

```php
public add_row_action(array $actions, \WP_Post $post): array
```

Adds a link to synchronize the product with the latest data from the BigCommerce API.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$actions` | **array** | The current list of actions available for the post. |
| `$post` | **\WP_Post** | The post object being viewed. |


**Return Value:**

Modified list of actions with the "Re-sync" link added.




***

### handle_request

Handles the request to sync the product when the sync URL is triggered.

```php
public handle_request(): void
```

Verifies the request and synchronizes the product with BigCommerce. Redirects to the appropriate page with a success or error message.










***


***
> Automatically generated on 2024-12-31
