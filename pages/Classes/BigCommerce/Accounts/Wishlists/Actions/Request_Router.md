***

# Request_Router

Class Request_Router

Routes incoming requests to the appropriate action handler for wishlist-related operations.

This class listens for requests on the wishlist action endpoint and directs them to the appropriate
handler based on the action specified in the request.

* Full name: `\BigCommerce\Accounts\Wishlists\Actions\Request_Router`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`ACTION`|public|string|&#039;wishlist&#039;|


## Methods


### handle_request

Handles the incoming request by routing it to the appropriate action handler.

```php
public handle_request(array $args): void
```

This method extracts the action from the request arguments, and then triggers a WordPress action
to handle the request using the specific action handler associated with the action.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | The arguments for the wishlist request, including the action and any parameters. |





***


***
> Automatically generated on 2025-01-13
