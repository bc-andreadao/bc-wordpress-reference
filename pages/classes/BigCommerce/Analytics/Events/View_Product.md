***

# View_Product

Class View_Product

Adds analytics events to product permalink and buttons for tracking.

This class is responsible for attaching analytics tracking attributes to the product's view
buttons and permalink. It tracks events such as product views by adding the necessary data
attributes to the HTML elements. The tracking includes product information like product ID,
name, and SKU if enabled in the settings.

* Full name: `\BigCommerce\Analytics\Events\View_Product`




## Methods


### add_tracking_attributes_to_button

Adds tracking attributes to the product view button.

```php
public add_tracking_attributes_to_button(array $options = [], string $template = &#039;&#039;): array
```

This function embeds tracking data into the attributes of the product view button.
The tracking attributes include product details like product ID, post ID, and product name.
It triggers the 'view_product' event when the button is clicked.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$options` | **array** | Options for the button. |
| `$template` | **string** | The template name for the button. |


**Return Value:**

Modified options with added tracking attributes.




***

### add_tracking_attributes_to_permalink

Adds tracking attributes to the product permalink.

```php
public add_tracking_attributes_to_permalink(array $options, string $template): array
```

This function attaches tracking data to the product permalink's attributes.
The tracking includes product details such as product ID, post ID, and product name.
The 'view_product' event is triggered when the permalink is clicked.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$options` | **array** | Options for the permalink. |
| `$template` | **string** | The template name for the permalink. |


**Return Value:**

Modified options with added tracking attributes.




***

### change_track_data

Updates tracking data to include SKU information if enabled in Analytics settings.

```php
public change_track_data(array $track_data): array
```

If SKU tracking is enabled in the Analytics options, this function appends the SKU
to the tracking data for the product. If a variant ID is provided, the variant's SKU
is also included. If the product cannot be loaded, the original tracking data is returned.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$track_data` | **array** | The existing tracking data. |


**Return Value:**

The updated tracking data, potentially including SKU information.




***


***
> Automatically generated on 2024-12-13
