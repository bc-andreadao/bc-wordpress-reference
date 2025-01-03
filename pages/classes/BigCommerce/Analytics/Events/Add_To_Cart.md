***

# Add_To_Cart

Class Add_To_Cart

Adds analytics tracking attributes to purchase buttons and success messages.

This class is responsible for enhancing the add-to-cart functionality by embedding
tracking attributes into the purchase buttons and success messages. The tracking
attributes are used to collect analytics data about the user's interactions.

* Full name: `\BigCommerce\Analytics\Events\Add_To_Cart`




## Methods


### set_tracking_attributes_on_success_message

Sets tracking attributes on the success message displayed after adding a product to the cart.

```php
public set_tracking_attributes_on_success_message(array $args, array $data): array
```

This function parses the data provided by the cart action and applies tracking attributes
to the success message. The tracking data includes details such as cart ID, product ID,
variant ID, and product name.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$args` | **array** | Attributes of the success message. |
| `$data` | **array** | Data related to the cart action. |


**Return Value:**

Modified success message attributes with tracking data.




***

### add_tracking_attributes_to_purchase_button

Adds tracking attributes to the purchase button for analytics purposes.

```php
public add_tracking_attributes_to_purchase_button(array $attributes, \BigCommerce\Post_Types\Product\Product $product): array
```

The tracking attributes include information about the product being purchased, such as
product ID, post ID, and product name. This data is embedded into the button's attributes
for tracking the add-to-cart action.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$attributes` | **array** | Attributes of the purchase button. |
| `$product` | **\BigCommerce\Post_Types\Product\Product** | The product object associated with the button. |


**Return Value:**

Modified button attributes with tracking data.




***


***
> Automatically generated on 2025-01-03
