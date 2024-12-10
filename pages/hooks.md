# Hooks

- [Actions](#actions)
- [Filters](#filters)

## Actions

### `pre_get_posts`

Modify the main query to filter products based on wishlist conditions.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`query` | `\WP_Query` | The main WordPress query object, which is filtered to show only wishlist-relevant products.

Source: [src/BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.php](BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.php), [line 76](BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.php#L76-L81)

### `pre_get_posts`

Adds a filter to modify the main query for filtering by channel.

This action is triggered on the `pre_get_posts` hook to apply a filter that
modifies the query to include the channel(s) based on the provided `$channel` parameter.

Checks if the specified channel
is valid and modify the query to filter by the valid channel IDs.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`query` | `\WP_Query` | The `WP_Query` object being modified. This is the main query that will be filtered by the channel ID(s).

Source: [src/BigCommerce/Rest/Products_Controller.php](BigCommerce/Rest/Products_Controller.php), [line 306](BigCommerce/Rest/Products_Controller.php#L306-L317)

### `bigcommerce/import/before`

Hook before the import starts.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`status` | `string` | Current status of the import.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 118](BigCommerce/CLI/Import_Products.php#L118-L125)

### `bigcommerce/import/after`

Hook after the import ends.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`status` | `string` | Final status after the import.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 127](BigCommerce/CLI/Import_Products.php#L127-L134)

### `bigcommerce/import/set_status`

Hook when the import status is set.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`status` | `string` | The status being set.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 136](BigCommerce/CLI/Import_Products.php#L136-L143)

### `bigcommerce/import/start`

Hook when the import starts.

**Arguments**

No arguments.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 145](BigCommerce/CLI/Import_Products.php#L145-L150)

### `bigcommerce/import/fetched_ids`

Hook after fetching product IDs.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`count` | `int` | Number of products added to the queue.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 152](BigCommerce/CLI/Import_Products.php#L152-L159)

### `bigcommerce/import/marked_deleted`

Hook after marking products for deletion.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`count` | `int` | Number of products marked for deletion.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 161](BigCommerce/CLI/Import_Products.php#L161-L168)

### `bigcommerce/import/product/created`

Hook when a product post is created.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_id` | `int` | The created post ID.
`data` | `array` | Product data.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 170](BigCommerce/CLI/Import_Products.php#L170-L178)

### `bigcommerce/import/product/updated`

Hook when a product post is updated.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_id` | `int` | The updated post ID.
`data` | `array` | Product data.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 180](BigCommerce/CLI/Import_Products.php#L180-L188)

### `bigcommerce/import/product/skipped`

Hook when a product post is skipped due to being up to date.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_id` | `int` | The skipped post ID.
`data` | `array` | Product data.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 190](BigCommerce/CLI/Import_Products.php#L190-L198)

### `bigcommerce/import/fetched_currency`

Hook after fetching currency code.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`currency_code` | `string` | The fetched currency code.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 200](BigCommerce/CLI/Import_Products.php#L200-L207)

### `bigcommerce/import/could_not_fetch_store_settings`

Hook when store settings cannot be fetched.

**Arguments**

No arguments.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 209](BigCommerce/CLI/Import_Products.php#L209-L214)

### `bigcommerce/import/error`

Hook when there is an import error.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`message` | `string` | Error message.
`data` | `array` | Additional error data.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 216](BigCommerce/CLI/Import_Products.php#L216-L227)

### `bigcommerce/import/product/error`

Hook when a product import fails.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`product_id` | `int` | The product ID.
`catalog_api` | `\BigCommerce\Api\v3\Api\CatalogApi` | The catalog API object.
`exception` | `\Exception` | The exception that occurred.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 229](BigCommerce/CLI/Import_Products.php#L229-L238)

### `bigcommerce/import/term/skipped`

Hook when a term import is skipped.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | Term data.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 240](BigCommerce/CLI/Import_Products.php#L240-L247)

### `admin_body_class`

Adds a custom body class to the admin panel.

This action hook adds a custom class to the admin body tag by calling the
`set_admin_body_class` method when the `admin_body_class` hook is triggered.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`classes` | `string` | The existing body classes.

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 175](BigCommerce/Settings/Screens/Abstract_Screen.php#L175-L185)

### `admin_menu`

Triggers an action for unregistered settings screens in the admin menu when the admin menu is loaded

This hook is intended to handle cases where settings
screens are not registered. The action is executed with a priority of 10000 to ensure
it's called after other actions have been triggered.

**Arguments**

No arguments.

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 490](BigCommerce/Settings/Screens/Abstract_Screen.php#L490-L501)

### `bigcommerce/channel/error/could_not_fetch_listing`

Handles errors when a listing cannot be fetched from the BigCommerce API.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`channel_id` | `int` | The channel ID.
`listing_id` | `int` | The listing ID.
`e` | `\BigCommerce\Api\v3\ApiException` | The exception thrown during the fetch attempt.

Source: [src/BigCommerce/Post_Types/Product/Reset_Listing.php](BigCommerce/Post_Types/Product/Reset_Listing.php), [line 167](BigCommerce/Post_Types/Product/Reset_Listing.php#L167-L174)

### `bigcommerce/channel/error/could_not_update_listing`

Handles errors when a listing update fails in the BigCommerce API.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`channel_id` | `int` | The channel ID.
`listing_id` | `int` | The listing ID.
`e` | `\BigCommerce\Api\v3\ApiException` | The exception thrown during the update attempt.

Source: [src/BigCommerce/Post_Types/Product/Reset_Listing.php](BigCommerce/Post_Types/Product/Reset_Listing.php), [line 176](BigCommerce/Post_Types/Product/Reset_Listing.php#L176-L183)

### `bigcommerce/import/error`

Adds an error handler for the 'bigcommerce/import/error' action hook.

This hook listens for errors during the product import process. If an error occurs, the handler adds
the error message to the `WP_Error` object for further processing.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`message` | `string` | The error message to be logged if the import fails.

Source: [src/BigCommerce/Post_Types/Product/Single_Product_Sync.php](BigCommerce/Post_Types/Product/Single_Product_Sync.php), [line 110](BigCommerce/Post_Types/Product/Single_Product_Sync.php#L110-L118)

### `admin_print_scripts-post.php`

Inline script added for the Gutenberg editor initialization.

**Arguments**

No arguments.

Source: [src/BigCommerce/Assets/Admin/Scripts.php](BigCommerce/Assets/Admin/Scripts.php), [line 83](BigCommerce/Assets/Admin/Scripts.php#L83-L88)

### `admin_print_footer_scripts`

Enqueue admin and Gutenberg scripts.

Registers and enqueues required scripts, and localizes them with configuration
and localization data. Delays certain script outputs until after the admin footer scripts.

**Arguments**

No arguments.

Source: [src/BigCommerce/Assets/Admin/Scripts.php](BigCommerce/Assets/Admin/Scripts.php), [line 47](BigCommerce/Assets/Admin/Scripts.php#L47-L99)

### `admin_footer-{$GLOBALS}[hook_suffix]`

Process the script queue again for the current admin footer.

**Arguments**

No arguments.

Source: [src/BigCommerce/Assets/Admin/Scripts.php](BigCommerce/Assets/Admin/Scripts.php), [line 113](BigCommerce/Assets/Admin/Scripts.php#L113-L116)

### `plugins_loaded`

Configures the static properties of the global V2 API client upon plugin load.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Api.php](BigCommerce/Container/Api.php), [line 231](BigCommerce/Container/Api.php#L231-L251)

### `update_option_Import_Settings::ENABLE_PRODUCTS_WEBHOOKS`

Triggered when the option to enable product webhooks is updated.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`old_value` | `mixed` | The previous value of the option.
`new_value` | `mixed` | The new value of the option.
`option_name` | `string` | The name of the option being updated.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 359](BigCommerce/Container/Webhooks.php#L359-L367)

### `add_option_Import_Settings::ENABLE_PRODUCTS_WEBHOOKS`

Listens for the addition of the product webhooks status option
and updates the webhook status accordingly.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`option_name` | `string` | The name of the option being added.
`value` | `mixed` | The value of the option being added.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 369](BigCommerce/Container/Webhooks.php#L369-L378)

### `update_option_Import_Settings::ENABLE_CUSTOMER_WEBHOOKS`

Triggers whenever the customer webhook enable/disable option
is updated, allowing related settings or functionalities to adjust.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`old_value` | `mixed` | The previous value of the option.
`new_value` | `mixed` | The new value of the option.
`option_name` | `string` | The name of the option being updated.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 391](BigCommerce/Container/Webhooks.php#L391-L401)

### `add_option_Import_Settings::ENABLE_CUSTOMER_WEBHOOKS`

Triggered when the customer webhook enable/disable option is added for the first time.

This allows related settings or functionalities to adjust when the option is initialized.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`option_name` | `string` | The name of the option being added.
`value` | `mixed` | The value of the option being added.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 403](BigCommerce/Container/Webhooks.php#L403-L415)

### `bigcommerce/settings/webhoooks_updated`

Triggered when webhook settings are updated in BigCommerce.

Ensures that the webhooks version is checked and updated as necessary.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 430](BigCommerce/Container/Webhooks.php#L430-L439)

### `bigcommerce/action_endpoint/webhook`

Handles incoming webhook requests from BigCommerce.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`args` | `array` | The request arguments received from the webhook.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 458](BigCommerce/Container/Webhooks.php#L458-L467)

### `bigcommerce/webhooks/customer_deleted`

Triggered when a customer is deleted via a webhook.

Handles customer deletion tasks based on the provided parameters.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`params` | `array` | An array of parameters containing details about the deleted customer.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 475](BigCommerce/Container/Webhooks.php#L475-L490)

### `bigcommerce/webhooks/customer_created`

Handles the "customer created" webhook event.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`customer_id` | `int` | The ID of the customer created.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 492](BigCommerce/Container/Webhooks.php#L492-L505)

### `bigcommerce/webhooks/customer_updated`

Triggered when a customer is updated via a webhook.

Updates the customer's information based on the provided ID.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`customer_id` | `int` | The ID of the customer being updated.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 507](BigCommerce/Container/Webhooks.php#L507-L522)

### `Customer_Channel_Webhook::HOOK`

Triggered when a customer's channel access is updated via a webhook.

Updates the customer's access to the specified channels.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`customer_id` | `int` | The ID of the customer.
`channels_id` | `array` | An array of channel IDs the customer has access to.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 524](BigCommerce/Container/Webhooks.php#L524-L540)

### `bigcommerce/webhooks/product_inventory_updated`

Handles the "product inventory updated" webhook event.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`params` | `array` | Parameters for the updated product, including product ID.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 555](BigCommerce/Container/Webhooks.php#L555-L569)

### `bigcommerce/webhooks/product_updated`

Handles the "product updated" webhook event.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`params` | `array` | The parameters of the updated product, including product ID.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 571](BigCommerce/Container/Webhooks.php#L571-L585)

### `bigcommerce/webhooks/product_deleted`

Triggered when a product is deleted via a webhook.

Handles product deletion tasks based on the provided parameters.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`params` | `array` | An array of parameters containing details about the deleted product.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 587](BigCommerce/Container/Webhooks.php#L587-L602)

### `bigcommerce/webhooks/product_created`

Triggered when a product is created via a webhook.

Handles the creation of a product based on the provided parameters.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`params` | `array` | An array of parameters containing details about the created product.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 604](BigCommerce/Container/Webhooks.php#L604-L619)

### `sprintf()`

Triggered when a product is assigned to a channel via a webhook.

Handles tasks related to assigning a product to a specific channel.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`product_id` | `int` | The ID of the product.
`channel_id` | `int` | The ID of the channel the product is assigned to.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 621](BigCommerce/Container/Webhooks.php#L621-L637)

### `sprintf()`

Triggered when a product is unassigned from a channel via a webhook.

Handles tasks related to unassigning a product from a specific channel.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`product_id` | `int` | The ID of the product.
`channel_id` | `int` | The ID of the channel the product is unassigned from.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 639](BigCommerce/Container/Webhooks.php#L639-L655)

### `Channels_Management_Webhook::CHANNEL_CURRENCY_UPDATE_HOOK`

Handles the "channel currency updated" webhook event.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`channel_id` | `int` | The ID of the channel whose currency was updated.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 657](BigCommerce/Container/Webhooks.php#L657-L670)

### `Channels_Management_Webhook::CHANNEL_UPDATED_HOOK`

Triggered when a channel is updated via a webhook.

Handles tasks related to updating channel details.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`channel_id` | `int` | The ID of the channel being updated.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 672](BigCommerce/Container/Webhooks.php#L672-L683)

### `Webhook_Cron_Tasks::UPDATE_PRODUCT`

Triggered by the cron task to update a product.

Handles the product update process for the specified product ID.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`product_id` | `int` | The ID of the product to update.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 695](BigCommerce/Container/Webhooks.php#L695-L706)

### `admin_init`

Ensures required pages exist during the `admin_init` action.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Pages.php](BigCommerce/Container/Pages.php), [line 211](BigCommerce/Container/Pages.php#L211-L221)

### `trashed_post`

Clears page options when a page is trashed.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_id` | `int` | The ID of the post being trashed.

Source: [src/BigCommerce/Container/Pages.php](BigCommerce/Container/Pages.php), [line 230](BigCommerce/Container/Pages.php#L230-L235)

### `deleted_post`

Clears page options when a page is deleted.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_id` | `int` | The ID of the post being deleted.

Source: [src/BigCommerce/Container/Pages.php](BigCommerce/Container/Pages.php), [line 237](BigCommerce/Container/Pages.php#L237-L242)

### `display_post_states`

Adds custom post states to display required pages in admin post lists.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_states` | `array` | Current post states.
`post` | `\BigCommerce\Container\WP_Post` | The current post object.

Source: [src/BigCommerce/Container/Pages.php](BigCommerce/Container/Pages.php), [line 244](BigCommerce/Container/Pages.php#L244-L257)

### `bigcommerce/settings/accounts/after_page_field/page=Registration_Page::NAME`

Adds a registration notice after the registration page field in settings.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Pages.php](BigCommerce/Container/Pages.php), [line 259](BigCommerce/Container/Pages.php#L259-L266)

### `the_content`

Filters the content of required pages.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`content` | `string` | The original page content.

Source: [src/BigCommerce/Container/Pages.php](BigCommerce/Container/Pages.php), [line 268](BigCommerce/Container/Pages.php#L268-L282)

### `template_redirect`

Action hook that checks for the presence of specific shortcodes (`Cart` and `Checkout`) during the template redirect and handles caching logic accordingly.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Cart.php](BigCommerce/Container/Cart.php), [line 179](BigCommerce/Container/Cart.php#L179-L189)

### `bigcommerce/do_not_cache`

Action hook that disables caching for cart and checkout pages.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Cart.php](BigCommerce/Container/Cart.php), [line 192](BigCommerce/Container/Cart.php#L192-L199)

### `bigcommerce/action_endpoint/Buy_Now::ACTION`

Action hook that handles the Buy Now request.

This hook is triggered when the `bigcommerce/action_endpoint/<ACTION>` endpoint
for the `Buy_Now` action is called. It processes the Buy Now request and handles
adding the item to the cart.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`args` | `array` | The arguments passed to the action (e.g., product details).

Source: [src/BigCommerce/Container/Cart.php](BigCommerce/Container/Cart.php), [line 207](BigCommerce/Container/Cart.php#L207-L220)

### `bigcommerce/action_endpoint/Add_To_Cart::ACTION`

Action hook that handles adding an item to the cart.

This hook is triggered when the `bigcommerce/action_endpoint/<ACTION>` endpoint
for the `Add_To_Cart` action is called. It processes the request to add an item to
the cart.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`args` | `array` | The arguments passed to the action (e.g., product details).

Source: [src/BigCommerce/Container/Cart.php](BigCommerce/Container/Cart.php), [line 232](BigCommerce/Container/Cart.php#L232-L245)

### `bigcommerce/action_endpoint/Cart_Recovery::ACTION`

Action hook that handles recovering an abandoned cart.

This hook is triggered when the `bigcommerce/action_endpoint/<ACTION>` endpoint
for the `Cart_Recovery` action is called. It processes the request to recover an
abandoned cart.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`args` | `array` | The arguments passed to the action (e.g., cart recovery data).

Source: [src/BigCommerce/Container/Cart.php](BigCommerce/Container/Cart.php), [line 247](BigCommerce/Container/Cart.php#L247-L260)

### `bigcommerce/action_endpoint/Checkout::ACTION`

Action hook that handles the checkout request.

This hook is triggered when the `bigcommerce/action_endpoint/<ACTION>` endpoint
for the `Checkout` action is called. It processes the checkout request and handles
the cart during the checkout process.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`args` | `array` | The arguments passed to the action (e.g., checkout data).

Source: [src/BigCommerce/Container/Cart.php](BigCommerce/Container/Cart.php), [line 288](BigCommerce/Container/Cart.php#L288-L301)

### `plugins_loaded`

Hook registers database tables during the `plugins_loaded` action.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Schema.php](BigCommerce/Container/Schema.php), [line 99](BigCommerce/Container/Schema.php#L99-L105)

### `admin_init`

Hook registers user roles during the `admin_init` action.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Schema.php](BigCommerce/Container/Schema.php), [line 141](BigCommerce/Container/Schema.php#L141-L146)

### `init`

Registers the custom action route during WordPress initialization.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Rewrites.php](BigCommerce/Container/Rewrites.php), [line 53](BigCommerce/Container/Rewrites.php#L53-L58)

### `parse_request`

Handles incoming requests for the custom action route.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`wp` | `\WP` | The WordPress environment instance containing the query vars.

Source: [src/BigCommerce/Container/Rewrites.php](BigCommerce/Container/Rewrites.php), [line 60](BigCommerce/Container/Rewrites.php#L60-L67)

### `wp_loaded`

Flushes rewrite rules after WordPress has fully loaded.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Rewrites.php](BigCommerce/Container/Rewrites.php), [line 80](BigCommerce/Container/Rewrites.php#L80-L85)

### `update_option_Product_Archive::ARCHIVE_SLUG`

Schedules a flush when the Product Archive Slug option is updated.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Rewrites.php](BigCommerce/Container/Rewrites.php), [line 94](BigCommerce/Container/Rewrites.php#L94-L97)

### `update_option_Product_Archive::CATEGORY_SLUG`

Schedules a flush when the Product Archive Category Slug option is updated.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Rewrites.php](BigCommerce/Container/Rewrites.php), [line 99](BigCommerce/Container/Rewrites.php#L99-L102)

### `update_option_Product_Archive::BRAND_SLUG`

Schedules a flush when the Product Archive Brand Slug option is updated.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Rewrites.php](BigCommerce/Container/Rewrites.php), [line 104](BigCommerce/Container/Rewrites.php#L104-L107)

### `add_option_Product_Archive::ARCHIVE_SLUG`

Schedules a flush when the Product Archive Slug option is added.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Rewrites.php](BigCommerce/Container/Rewrites.php), [line 109](BigCommerce/Container/Rewrites.php#L109-L112)

### `add_option_Product_Archive::CATEGORY_SLUG`

Schedules a flush when the Product Archive Category Slug option is added.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Rewrites.php](BigCommerce/Container/Rewrites.php), [line 114](BigCommerce/Container/Rewrites.php#L114-L117)

### `add_option_Product_Archive::BRAND_SLUG`

Schedules a flush when the Product Archive Brand Slug option is added.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Rewrites.php](BigCommerce/Container/Rewrites.php), [line 119](BigCommerce/Container/Rewrites.php#L119-L122)

### `after_setup_theme`

Hook registers all WordPress shortcodes during the `after_setup_theme` action.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Shortcodes.php](BigCommerce/Container/Shortcodes.php), [line 174](BigCommerce/Container/Shortcodes.php#L174-L191)

### `customize_register`

Registers customizer panels and sections in WordPress.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`wp_customize` | `\WP_Customize_Manager` | The WordPress Customizer manager instance.

Source: [src/BigCommerce/Container/Theme_Customizer.php](BigCommerce/Container/Theme_Customizer.php), [line 167](BigCommerce/Container/Theme_Customizer.php#L167-L188)

### `wp_head`

Outputs customizer styles in the WordPress head section.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Theme_Customizer.php](BigCommerce/Container/Theme_Customizer.php), [line 190](BigCommerce/Container/Theme_Customizer.php#L190-L195)

### `admin_menu`

Registers the settings screen in the WordPress admin menu.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 357](BigCommerce/Container/Settings.php#L357-L363)

### `bigcommerce/settings/after_form/page=Settings_Screen::NAME`

Adds a support message after the settings form for the specific settings page.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `array` | Dependency injection container.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 374](BigCommerce/Container/Settings.php#L374-L381)

### `admin_init`

Redirects to the settings screen upon plugin activation.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 426](BigCommerce/Container/Settings.php#L426-L435)

### `bigcommerce/settings/register/screen=Settings_Screen::NAME`

Registers settings for a specific screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`screen` | `string` | The screen identifier.
`settings` | `array` | The settings to register.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 447](BigCommerce/Container/Settings.php#L447-L453)

### `bigcommerce/settings/register/screen=Api_Credentials_Screen::NAME`

Registers settings for a specific screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`screen` | `string` | The screen identifier.
`settings` | `array` | The settings to register.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 455](BigCommerce/Container/Settings.php#L455-L461)

### `bigcommerce/settings/render/credentials`

Renders API credentials description for the credentials section.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `array` | Dependency injection container.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 463](BigCommerce/Container/Settings.php#L463-L470)

### `update_option_Api_Credentials::OPTION_STORE_URL`

Performs actions after an API credential option is updated.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`old_value` | `mixed` | The old option value.
`value` | `mixed` | The new option value.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 590](BigCommerce/Container/Settings.php#L590-L596)

### `update_option_Api_Credentials::OPTION_CLIENT_ID`

Performs actions after an API credential option is updated.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`old_value` | `mixed` | The old option value.
`value` | `mixed` | The new option value.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 598](BigCommerce/Container/Settings.php#L598-L604)

### `update_option_Api_Credentials::OPTION_CLIENT_SECRET`

Performs actions after an API credential option is updated.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`old_value` | `mixed` | The old option value.
`value` | `mixed` | The new option value.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 606](BigCommerce/Container/Settings.php#L606-L612)

### `update_option_Api_Credentials::OPTION_ACCESS_TOKEN`

Performs actions after an API credential option is updated.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`old_value` | `mixed` | The old option value.
`value` | `mixed` | The new option value.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 614](BigCommerce/Container/Settings.php#L614-L620)

### `admin_notices`

Adds a notice for credentials required on certain admin screens.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 628](BigCommerce/Container/Settings.php#L628-L646)

### `bigcommerce/settings/register/screen=Settings_Screen::NAME`

Registers API status settings and flushes the status cache on load.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`hook` | `string` | The screen hook suffix.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 652](BigCommerce/Container/Settings.php#L652-L663)

### `load-{$hook}`

Flushes the API status cache.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 659](BigCommerce/Container/Settings.php#L659-L662)

### `bigcommerce/settings/register/screen=Settings_Screen::NAME`

Registers cart settings section.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 672](BigCommerce/Container/Settings.php#L672-L677)

### `bigcommerce/settings/register/screen=Settings_Screen::NAME`

Registers gift certificate settings section.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 690](BigCommerce/Container/Settings.php#L690-L695)

### `bigcommerce/settings/register/screen=Settings_Screen::NAME`

Registers the settings section for the import functionality on the settings screen.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 711](BigCommerce/Container/Settings.php#L711-L714)

### `bigcommerce/settings/register/screen=Connect_Channel_Screen::NAME`

Registers the fields for connecting channels to the import functionality on the settings screen.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 716](BigCommerce/Container/Settings.php#L716-L721)

### `bigcommerce/settings/header/import_status`

Renders the import button in the settings header.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 727](BigCommerce/Container/Settings.php#L727-L732)

### `admin_post_Import_Now::ACTION`

Handles the import request from the admin panel.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 749](BigCommerce/Container/Settings.php#L749-L752)

### `admin_notices`

Displays import notices in the admin area if the import process is complete.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 754](BigCommerce/Container/Settings.php#L754-L761)

### `bigcommerce/settings/section/after_fields/id=Import_Settings::NAME`

Renders the import status after the fields section in the settings screen.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 773](BigCommerce/Container/Settings.php#L773-L776)

### `bigcommerce/settings/before_title/page=Onboarding_Complete_Screen::NAME`

Renders the import status before the title on the onboarding complete screen.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 778](BigCommerce/Container/Settings.php#L778-L781)

### `bigcommerce/settings/import/product_list_table_notice`

Displays the current import status notice in the product list table.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 783](BigCommerce/Container/Settings.php#L783-L790)

### `bigcommerce/import/before`

Caches the import queue size before initiating the import process, if certain product statuses
are marked for deletion.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`status` | `string` | The current status of the import process.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 792](BigCommerce/Container/Settings.php#L792-L802)

### `wp_ajax_Import_Status::AJAX_ACTION_IMPORT_STATUS`

This hook is triggered during an AJAX call to validate the current status
of the import process. It ensures that the request is valid and checks
the current state of the import.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 805](BigCommerce/Container/Settings.php#L805-L812)

### `wp_ajax_Import_Status::AJAX_ACTION_IMPORT_STATUS`

Handles the current status message for the import process via an AJAX request.

This hook responds to an AJAX request by providing the current status
message of the import process. It ensures the user gets real-time feedback
during import operations.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 815](BigCommerce/Container/Settings.php#L815-L824)

### `update_option_Import_Settings::HEADLESS_FLAG`

Switches import behavior when the headless flag is updated. It adjusts the import behavior based on the new value of the flag.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`old_value` | `mixed` | The old value of the option.
`new_value` | `mixed` | The new value of the option.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 826](BigCommerce/Container/Settings.php#L826-L833)

### `bigcommerce/settings/register/screen=Settings_Screen::NAME`

Registers the currency settings section in the BigCommerce settings screen.

This hook adds a currency settings section to the BigCommerce settings
screen, allowing configuration of currency-related settings.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 841](BigCommerce/Container/Settings.php#L841-L849)

### `bigcommerce/settings/register/screen=Settings_Screen::NAME`

Registers the "Next Steps" section in the BigCommerce settings screen.

This hook adds a "Next Steps" section to the BigCommerce settings screen,
providing guidance for merchants on the next steps in setting up their store.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 859](BigCommerce/Container/Settings.php#L859-L867)

### `bigcommerce/settings/register/screen=Settings_Screen::NAME`

Registers the account settings section in the BigCommerce settings screen.

This hook adds an account settings section to the BigCommerce settings screen,
allowing configuration of account-related settings such as login, registration,
and user-specific pages.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 885](BigCommerce/Container/Settings.php#L885-L894)

### `init`

Adds default global logins during the initialization phase.

This hook ensures that the default global login settings are added to
the account configuration when the system initializes.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 896](BigCommerce/Container/Settings.php#L896-L904)

### `update_option_Account_Settings::ALLOW_GLOBAL_LOGINS`

Synchronizes global logins when the "Allow Global Logins" setting is updated.

This hook is triggered when the "Allow Global Logins" option is updated. It
synchronizes the global login settings based on the new value.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`old_value` | `mixed` | The previous value of the global logins setting.
`new_value` | `mixed` | The updated value of the global logins setting.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 906](BigCommerce/Container/Settings.php#L906-L917)

### `bigcommerce/settings/register/screen=Settings_Screen::NAME`

Registers the analytics settings section in the BigCommerce settings screen.

This hook adds an analytics settings section to the BigCommerce settings screen,
allowing configuration of analytics-related settings like Facebook Pixel and Google Analytics.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 925](BigCommerce/Container/Settings.php#L925-L933)

### `update_option_Analytics_Settings::FACEBOOK_PIXEL`

Updates the Facebook Pixel ID when the setting is updated.

This hook triggers when the Facebook Pixel ID setting is updated and updates the
associated analytics section.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`old_value` | `mixed` | The previous value of the Facebook Pixel ID.
`new_value` | `mixed` | The new value of the Facebook Pixel ID.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 935](BigCommerce/Container/Settings.php#L935-L946)

### `update_option_Analytics_Settings::GOOGLE_ANALYTICS`

Updates the Google Analytics setting when the option is updated.

This hook triggers when the Google Analytics setting is updated and updates
the associated analytics section.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`old_value` | `mixed` | The previous value of the Google Analytics setting.
`new_value` | `mixed` | The new value of the Google Analytics setting.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 948](BigCommerce/Container/Settings.php#L948-L959)

### `bigcommerce/settings/register/screen=Settings_Screen::NAME`

Registers the reviews settings section in the BigCommerce settings screen.

This hook adds a reviews settings section to the BigCommerce settings screen,
allowing configuration of product review settings.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 968](BigCommerce/Container/Settings.php#L968-L976)

### `admin_menu`

Registers the welcome screen settings page in the admin menu.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 986](BigCommerce/Container/Settings.php#L986-L993)

### `admin_menu`

Registers the create account screen settings page in the admin menu.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The container instance holding the service dependencies.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1016](BigCommerce/Container/Settings.php#L1016-L1024)

### `admin_post_Create_Account_Screen::NAME`

Handles the submission for creating a BigCommerce account.

This action is triggered when a user submits the form to create a new BigCommerce account.
It processes the request and handles the form submission logic.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1039](BigCommerce/Container/Settings.php#L1039-L1049)

### `bigcommerce/settings/register/screen=Create_Account_Screen::NAME`

Registers a new account section for the Create Account screen.

This action is triggered to register a new account section for the Create Account screen
in the BigCommerce settings.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1051](BigCommerce/Container/Settings.php#L1051-L1061)

### `bigcommerce/create_account/validate_request`

Validates the request for creating a new BigCommerce account.

This action is triggered when a request is made to create a new account. It validates
the submission data and checks for any errors before processing the request.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`submission` | `array` | The submitted data from the account creation form.
`errors` | `array` | The array of validation errors, if any.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1063](BigCommerce/Container/Settings.php#L1063-L1075)

### `admin_menu`

Registers the Store Type screen in the BigCommerce settings menu.

This action is triggered to display the Store Type screen during the BigCommerce
onboarding process, where users can select the type of store they want to set up.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1077](BigCommerce/Container/Settings.php#L1077-L1087)

### `admin_post_Store_Type_Screen::ACTION_BLOG`

Handles the submission for choosing the blog store type.

This action is triggered when a user selects the blog store type during the
BigCommerce onboarding process. It processes the submission and updates the store configuration.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1089](BigCommerce/Container/Settings.php#L1089-L1099)

### `admin_post_Store_Type_Screen::ACTION_FULL_STORE`

Handles the submission for choosing the full store type.

This action is triggered when a user selects the full store type during the
BigCommerce onboarding process. It processes the submission and updates the store configuration.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1101](BigCommerce/Container/Settings.php#L1101-L1111)

### `admin_menu`

Registers the Channel screen in the BigCommerce settings menu.

This action is triggered to display the Channel selection screen during the BigCommerce
onboarding process, where users can connect a store channel.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1113](BigCommerce/Container/Settings.php#L1113-L1123)

### `bigcommerce/settings/register/screen=Connect_Channel_Screen::NAME`

Registers settings sections for selecting channels and importing settings.

This action is triggered to register settings sections for the Channel setup
and Onboarding Import Settings sections.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1125](BigCommerce/Container/Settings.php#L1125-L1136)

### `bigcommerce/settings/register/screen=Settings_Screen::NAME`

Registers the Channel Settings section in the BigCommerce settings menu.

This action is triggered to register the Channel Settings section for the
Settings Screen, where users can configure their channels.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1138](BigCommerce/Container/Settings.php#L1138-L1148)

### `admin_post_Channel_Settings::POST_ACTION`

Handles the channel operation actions in the settings screen.

This action is triggered when a channel operation is submitted in the BigCommerce settings.
It processes the submitted action and updates the channel configuration.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1150](BigCommerce/Container/Settings.php#L1150-L1162)

### `bigcommerce/channel/promote`

Promotes a channel in the BigCommerce settings.

This action is triggered when a channel is promoted in the BigCommerce settings. It
updates the channel configuration to reflect the promotion status.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`term` | `\WP_Term` | The channel term being promoted.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1164](BigCommerce/Container/Settings.php#L1164-L1175)

### `admin_menu`

Registers the Pending Account screen in the BigCommerce settings menu.

This action is triggered to display the Pending Account screen during the BigCommerce
onboarding process, which provides users with a pending account notification.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1177](BigCommerce/Container/Settings.php#L1177-L1187)

### `admin_menu`

Registers the API Credentials screen in the admin menu.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The container instance holding the service dependencies.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1205](BigCommerce/Container/Settings.php#L1205-L1213)

### `admin_action_update`

Handles the validation of API credentials during the admin action update.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The container instance holding the service dependencies.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1226](BigCommerce/Container/Settings.php#L1226-L1234)

### `admin_menu`

Provides various screens and settings for BigCommerce.

This class is responsible for registering settings screens, handling API credentials,
and managing various onboarding steps in the BigCommerce plugin.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 51](BigCommerce/Container/Settings.php#L51-L1247)

### `admin_menu`

Provides various screens and settings for BigCommerce.

This class is responsible for registering settings screens, handling API credentials,
and managing various onboarding steps in the BigCommerce plugin.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 51](BigCommerce/Container/Settings.php#L51-L1262)

### `bigcommerce/settings/register/screen=Nav_Menu_Screen::NAME`

Provides various screens and settings for BigCommerce.

This class is responsible for registering settings screens, handling API credentials,
and managing various onboarding steps in the BigCommerce plugin.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 51](BigCommerce/Container/Settings.php#L51-L1274)

### `admin_post_Nav_Menu_Screen::NAME`

Handles the submission of the Nav Menu setup screen.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1276](BigCommerce/Container/Settings.php#L1276-L1283)

### `bigcommerce/settings/unregistered_screen`

Redirects to the appropriate screen when an unregistered screen is encountered.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`unregistered_screen` | `string` | The name of the unregistered screen.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1285](BigCommerce/Container/Settings.php#L1285-L1307)

### `bigcommerce/settings/after_form/page=Api_Credentials_Screen::NAME`

Registers a callback function to be executed after the form on the API credentials screen. The callback adds a "start over" link to the settings screen.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1318](BigCommerce/Container/Settings.php#L1318-L1319)

### `bigcommerce/settings/after_form/page=Create_Account_Screen::NAME`

Registers a callback function to be executed after the form on the create account screen. The callback adds a "start over" link to the settings screen.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1320](BigCommerce/Container/Settings.php#L1320-L1321)

### `bigcommerce/settings/after_form/page=Connect_Channel_Screen::NAME`

Registers a callback function to be executed after the form on the connect channel screen. The callback adds a "start over" link to the settings screen.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1322](BigCommerce/Container/Settings.php#L1322-L1323)

### `bigcommerce/settings/after_form/page=Store_Type_Screen::NAME`

Registers a callback function to be executed after the form on the store type screen. The callback adds a "start over" link to the settings screen.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1324](BigCommerce/Container/Settings.php#L1324-L1325)

### `bigcommerce/settings/after_content/page=Pending_Account_Screen::NAME`

Registers a callback function to be executed after the form on the pending account screen. The callback adds a "start over" link to the settings screen.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1326](BigCommerce/Container/Settings.php#L1326-L1327)

### `admin_post_Start_Over::ACTION`

Resets the credentials when the "start over" action is triggered.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1329](BigCommerce/Container/Settings.php#L1329-L1332)

### `bigcommerce/settings/onboarding/progress`

Registers a callback to render the onboarding progress bar on the 'bigcommerce/settings/onboarding/progress' hook.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`progress_bar` | `callable` | The callback function to render the progress bar.
`priority` | `int` | The priority at which the callback should be executed. Defaults to 10.
`accepted_args` | `int` | The number of arguments the callback accepts. Defaults to 0.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1350](BigCommerce/Container/Settings.php#L1350-L1358)

### `bigcommerce/settings/before_title/page=Welcome_Screen::NAME`

Registers a callback to display the onboarding subheader before the title on the Welcome screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`subheader` | `callable` | The callback function to display the subheader.
`priority` | `int` | The priority at which the callback should be executed. Defaults to 10.
`accepted_args` | `int` | The number of arguments the callback accepts. Defaults to 0.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1364](BigCommerce/Container/Settings.php#L1364-L1372)

### `bigcommerce/settings/before_title/page=Create_Account_Screen::NAME`

Registers a callback to display the onboarding subheader before the title on the Create Account screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`subheader` | `callable` | The callback function to display the subheader.
`priority` | `int` | The priority at which the callback should be executed. Defaults to 10.
`accepted_args` | `int` | The number of arguments the callback accepts. Defaults to 0.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1374](BigCommerce/Container/Settings.php#L1374-L1382)

### `bigcommerce/settings/before_title/page=Api_Credentials_Screen::NAME`

Registers a callback to display the onboarding subheader before the title on the API Credentials screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`subheader` | `callable` | The callback function to display the subheader.
`priority` | `int` | The priority at which the callback should be executed. Defaults to 10.
`accepted_args` | `int` | The number of arguments the callback accepts. Defaults to 0.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1384](BigCommerce/Container/Settings.php#L1384-L1392)

### `bigcommerce/settings/before_title/page=Pending_Account_Screen::NAME`

Registers a callback to display the onboarding subheader before the title on the Pending Account screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`subheader` | `callable` | The callback function to display the subheader.
`priority` | `int` | The priority at which the callback should be executed. Defaults to 10.
`accepted_args` | `int` | The number of arguments the callback accepts. Defaults to 0.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1394](BigCommerce/Container/Settings.php#L1394-L1402)

### `bigcommerce/settings/before_title/page=Connect_Channel_Screen::NAME`

Registers a callback to display the onboarding subheader before the title on the Connect Channel screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`subheader` | `callable` | The callback function to display the subheader.
`priority` | `int` | The priority at which the callback should be executed. Defaults to 10.
`accepted_args` | `int` | The number of arguments the callback accepts. Defaults to 0.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1404](BigCommerce/Container/Settings.php#L1404-L1412)

### `bigcommerce/settings/before_title/page=Store_Type_Screen::NAME`

Registers a callback to display the onboarding subheader before the title on the Store Type screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`subheader` | `callable` | The callback function to display the subheader.
`priority` | `int` | The priority at which the callback should be executed. Defaults to 10.
`accepted_args` | `int` | The number of arguments the callback accepts. Defaults to 0.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1414](BigCommerce/Container/Settings.php#L1414-L1422)

### `bigcommerce/settings/before_title/page=Nav_Menu_Screen::NAME`

Registers a callback to display the onboarding subheader before the title on the Navigation Menu screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`subheader` | `callable` | The callback function to display the subheader.
`priority` | `int` | The priority at which the callback should be executed. Defaults to 10.
`accepted_args` | `int` | The number of arguments the callback accepts. Defaults to 0.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1424](BigCommerce/Container/Settings.php#L1424-L1432)

### `load-nav-menus.php`

Registers a callback to set the navigation menu screen options when the 'load-nav-menus.php' hook is triggered.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1445](BigCommerce/Container/Settings.php#L1445-L1451)

### `bigcommerce/settings/register/screen=Settings_Screen::NAME`

Registers a callback to register diagnostics settings on the 'bigcommerce/settings/register/screen=' hook for the specified screen.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1475](BigCommerce/Container/Settings.php#L1475-L1478)

### `wp_ajax_Troubleshooting_Diagnostics::AJAX_ACTION`

Registers a callback to handle diagnostics data retrieval for the specified AJAX action.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1480](BigCommerce/Container/Settings.php#L1480-L1483)

### `wp_ajax_Troubleshooting_Diagnostics::AJAX_ACTION_IMPORT_ERRORS`

Registers a callback to handle import errors retrieval for the specified AJAX action.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1485](BigCommerce/Container/Settings.php#L1485-L1488)

### `admin_post_Troubleshooting_Diagnostics::SYNC_SITE_URL`

Registers a callback to sync the site URL when the admin post action is triggered.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1490](BigCommerce/Container/Settings.php#L1490-L1493)

### `admin_post_Troubleshooting_Diagnostics::ABORT_NAME`

Registers a callback to abort the import when the admin post action is triggered.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1495](BigCommerce/Container/Settings.php#L1495-L1498)

### `admin_post_Troubleshooting_Diagnostics::FLUSH_USER`

Registers a callback to handle cache flush requests for the user.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1504](BigCommerce/Container/Settings.php#L1504-L1505)

### `admin_post_Troubleshooting_Diagnostics::FLUSH_PRODUCTS`

Registers a callback to handle cache flush requests for the products.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1506](BigCommerce/Container/Settings.php#L1506-L1507)

### `admin_menu`

Registers the resources settings page in the admin menu.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1517](BigCommerce/Container/Settings.php#L1517-L1520)

### `init`

Registers the necessary post types and handlers during the 'init' action.

This action is triggered on the 'init' hook to register several post types and
related configurations, including the product post type, queue task, synchronization logs,
and GraphQL product handlers. These handlers are instantiated from the container and
are responsible for managing product data, tasks, synchronization, and GraphQL operations.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 128](BigCommerce/Container/Post_Types.php#L128-L143)

### `pre_get_posts`

Action triggered before WordPress queries are retrieved to filter product queries.

This action hooks into the `pre_get_posts` event and modifies the query by filtering
it using the `filter_queries` method of the `PRODUCT_QUERY` container instance.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`query` | `\WP_Query` | The WordPress query object to be modified.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 185](BigCommerce/Container/Post_Types.php#L185-L197)

### `pre_handle_404`

Action triggered before the 404 handler to filter non-visible product categories.

This action hooks into the `pre_handle_404` event to handle non-visible product categories
by checking if the current category or archive is visible based on the setting in the customizer.
If the category is non-visible, it returns a 404 response.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`preempt` | `bool` | Whether the 404 handling should be preempted.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 227](BigCommerce/Container/Post_Types.php#L227-L263)

### `add_meta_boxes_Product\Product::NAME`

Action triggered to remove the featured image meta box for product posts.

This action hooks into the `add_meta_boxes_{post_type}` event and removes the featured
image meta box from the product post type using the `remove_featured_image_meta_box` method
of the `PRODUCT_ADMIN` container instance.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post` | `\WP_Post` | The post object for which the meta box is being added.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 304](BigCommerce/Container/Post_Types.php#L304-L317)

### `load-post.php`

Action triggered on the 'load-post.php' hook to initialize post admin functionalities.

This action triggers the `$load_post_admin_hooks` callback when loading the `post.php` page in the WordPress admin
to initialize various post-related admin functionalities.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 322](BigCommerce/Container/Post_Types.php#L322-L330)

### `wp_ajax_inline-save`

Action triggered on the 'wp_ajax_inline-save' hook to handle inline post saving functionality.

This action triggers the `$load_post_admin_hooks` callback during an AJAX request to save a post inline.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 332](BigCommerce/Container/Post_Types.php#L332-L339)

### `load-edit.php`

Action triggered on the 'load-edit.php' hook to initialize the post editing page admin functionalities.

This action triggers the `$load_post_admin_hooks` callback when loading the `edit.php` page in the WordPress admin
to initialize various editing-related functionalities.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 341](BigCommerce/Container/Post_Types.php#L341-L349)

### `rest_api_init`

Action triggered on the 'rest_api_init' hook to initialize REST API routes for post handling.

This action triggers the `$load_post_admin_hooks` callback during the REST API initialization process.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 351](BigCommerce/Container/Post_Types.php#L351-L358)

### `admin_notices`

Action triggered to show admin notices in the product list table.

This action is used to display admin notices in the product list table using the `list_table_admin_notices` method.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 426](BigCommerce/Container/Post_Types.php#L426-L435)

### `before_delete_post`

Action triggered before deleting a product to clean up associated data.

This action is triggered before a product is deleted, allowing for the removal of any associated product data
using the `delete_product_data` method.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_id` | `int` | The ID of the post being deleted.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 481](BigCommerce/Container/Post_Types.php#L481-L493)

### `bigcommerce/import/before`

Action triggered before the BigCommerce import process begins to disable updates.

This action disables updates or deletions of product listings in BigCommerce during the import process.
Do not push updates back upstream when running an import.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 495](BigCommerce/Container/Post_Types.php#L495-L506)

### `bigcommerce/import/after`

Action triggered after the BigCommerce import process to re-enable updates.

This action re-enables the updates and deletions of product listings in BigCommerce after the import process.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 508](BigCommerce/Container/Post_Types.php#L508-L518)

### `manage_bigcommerce_product_posts_custom_column`

Adds BigCommerce product ID values to custom columns in the admin product list.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`columns` | `array` | The existing columns in the admin product list.
`post_id` | `int` | The post ID.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 533](BigCommerce/Container/Post_Types.php#L533-L543)

### `manage_bigcommerce_product_posts_custom_column`

Adds BigCommerce product thumbnail image to custom columns in the admin product list.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`columns` | `array` | The existing columns in the admin product list.
`post_id` | `int` | The post ID.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 545](BigCommerce/Container/Post_Types.php#L545-L555)

### `bigcommerce/import/start`

Creates a sync entry when an import starts.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`error` | `string` | Error message (if any).

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 596](BigCommerce/Container/Post_Types.php#L596-L607)

### `bigcommerce/import/error`

Logs an error during the import process.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`error` | `string` | Error message encountered during the import process.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 609](BigCommerce/Container/Post_Types.php#L609-L620)

### `bigcommerce/import/logs/rotate`

Completes the sync when the logs are rotated.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`log` | `string` | The log data.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 622](BigCommerce/Container/Post_Types.php#L622-L633)

### `admin_bar_menu`

Modifies the admin bar links for editing products.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`wp_admin_bar` | `\BigCommerce\Container\WP_Admin_Bar` | The admin bar instance.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 701](BigCommerce/Container/Post_Types.php#L701-L712)

### `admin_post_Product\Reset_Listing::ACTION`

Handles the reset listing request via an admin action.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 741](BigCommerce/Container/Post_Types.php#L741-L750)

### `admin_post_Product\Single_Product_Sync::ACTION`

Handles product resync on admin post action.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 777](BigCommerce/Container/Post_Types.php#L777-L784)

### `post_submitbox_misc_actions`

Adds a channel indicator message in the post submitbox.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post` | `\BigCommerce\Container\WP_Post` | The post object.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 799](BigCommerce/Container/Post_Types.php#L799-L810)

### `save_post`

Syncs post data to an external channel when the post is saved.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_id` | `int` | The post ID.
`post` | `\BigCommerce\Container\WP_Post` | The post object.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 840](BigCommerce/Container/Post_Types.php#L840-L850)

### `before_delete_post`

Deletes post data from an external channel when the post is deleted.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_id` | `int` | The post ID.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 852](BigCommerce/Container/Post_Types.php#L852-L861)

### `widgets_init`

Registers each widget in the container during the `widgets_init` action.

This action hooks into `widgets_init` to register the defined widgets with WordPress.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`` | `void` | 

Source: [src/BigCommerce/Container/Widgets.php](BigCommerce/Container/Widgets.php), [line 41](BigCommerce/Container/Widgets.php#L41-L54)

### `wp_login`

Action hook to connect customer ID after successful login.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`username` | `string` | Username of the logged-in user
`user` | `\BigCommerce\Container\WP_User` | The WP user object

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 216](BigCommerce/Container/Accounts.php#L216-L224)

### `lostpassword_post`

Action hook for handling lost password errors.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`error` | `\WP_Error` | Error object from the lost password process.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 271](BigCommerce/Container/Accounts.php#L271-L278)

### `template_redirect`

Redirect account pages to authentication pages and vice versa.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 290](BigCommerce/Container/Accounts.php#L290-L296)

### `user_register`

Action hook for creating a customer when a new user registers.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`user_id` | `int` | The new user ID.
`userdata` | `array` | The user data.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 331](BigCommerce/Container/Accounts.php#L331-L339)

### `show_user_profile`

Registers profile-related services and actions.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The dependency injection container

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 392](BigCommerce/Container/Accounts.php#L392-L431)

### `edit_user_profile`

Registers profile-related services and actions.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The dependency injection container

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 392](BigCommerce/Container/Accounts.php#L392-L432)

### `personal_options_update`

Registers profile-related services and actions.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The dependency injection container

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 392](BigCommerce/Container/Accounts.php#L392-L433)

### `edit_user_profile_update`

Registers profile-related services and actions.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The dependency injection container

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 392](BigCommerce/Container/Accounts.php#L392-L434)

### `parse_request`

Action to handle address deletion requests

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 448](BigCommerce/Container/Accounts.php#L448-L451)

### `parse_request`

Action to handle public wishlist requests

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 482](BigCommerce/Container/Accounts.php#L482-L485)

### `bigcommerce/action_endpoint/Wishlist_Actions\Request_Router::ACTION`

Handle the wishlist action request

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 492](BigCommerce/Container/Accounts.php#L492-L495)

### `bigcommerce/wishlist_endpoint/Wishlist_Actions\Create_Wishlist::ACTION`

Handle create wishlist request

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 502](BigCommerce/Container/Accounts.php#L502-L505)

### `bigcommerce/wishlist_endpoint/Wishlist_Actions\Edit_Wishlist::ACTION`

Handle edit wishlist request

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 512](BigCommerce/Container/Accounts.php#L512-L515)

### `bigcommerce/wishlist_endpoint/Wishlist_Actions\Delete_Wishlist::ACTION`

Handle delete wishlist request

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 522](BigCommerce/Container/Accounts.php#L522-L525)

### `bigcommerce/wishlist_endpoint/Wishlist_Actions\Add_Item::ACTION`

Handle add item to wishlist request

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 532](BigCommerce/Container/Accounts.php#L532-L535)

### `bigcommerce/wishlist_endpoint/Wishlist_Actions\Remove_Item::ACTION`

Handle remove item from wishlist request

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 542](BigCommerce/Container/Accounts.php#L542-L545)

### `bigcommerce/template=components/products/product-single.php/data`

Registers and handles wishlist-related services and actions.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The dependency injection container

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 471](BigCommerce/Container/Accounts.php#L471-L556)

### `after_password_reset`

Sync password reset with BigCommerce

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 571](BigCommerce/Container/Accounts.php#L571-L574)

### `profile_update`

Sync password change with BigCommerce

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 576](BigCommerce/Container/Accounts.php#L576-L579)

### `bigcommerce/sync_global_logins`

Sync global logins with BigCommerce

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 592](BigCommerce/Container/Accounts.php#L592-L595)

### `bigcommerce/channel/promote`

Schedule global logins sync

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 597](BigCommerce/Container/Accounts.php#L597-L600)

### `parse_request`

Parses incoming requests and triggers the corresponding form action
when the `bc-action` parameter is present. Dynamically fires
a `bigcommerce/form/action=<action>` hook based on the value of `bc-action`.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 122](BigCommerce/Container/Forms.php#L122-L132)

### `bigcommerce/form/action=Delete_Address_Handler::ACTION`

Triggered when the form submission specifies `delete_address` as the `bc-action` parameter.

Handles the removal of an address from the user's account.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`submission` | `array` | The sanitized form submission data containing details for the address to be deleted.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 138](BigCommerce/Container/Forms.php#L138-L146)

### `bigcommerce/form/action=Update_Address_Handler::ACTION`

Triggered when the form submission specifies `update_address` as the `bc-action` parameter.

Handles updating an existing address in the user account by processing and validating the form data.
Developers can hook into this action to extend or customize address update behavior.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`submission` | `array` | The sanitized form submission data (typically from $_POST), containing user-provided fields for the address update.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 152](BigCommerce/Container/Forms.php#L152-L161)

### `bigcommerce/form/action=Update_Profile_Handler::ACTION`

Triggered when the form submission specifies `update_profile` as the `bc-action` parameter.

Handles updates to the user's profile details, such as name or email address.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`submission` | `array` | The sanitized form submission data containing user profile fields to be updated.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 167](BigCommerce/Container/Forms.php#L167-L175)

### `bigcommerce/form/action=Registration_Handler::ACTION`

Triggered when the form submission specifies `register` as the `bc-action` parameter.

Handles user registration by validating input data and creating a new account.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`submission` | `array` | The sanitized form submission data containing user registration details such as name, email, and password.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 181](BigCommerce/Container/Forms.php#L181-L189)

### `bigcommerce/form/action=Purchase_Gift_Certificate_Handler::ACTION`

Triggered when the form submission specifies `purchase_gift_certificate` as the `bc-action` parameter.

Handles the purchase of a gift certificate by processing user input and creating a cart item.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`submission` | `array` | The sanitized form submission data containing gift certificate purchase details.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 195](BigCommerce/Container/Forms.php#L195-L203)

### `bigcommerce/form/action=Product_Review_Handler::ACTION`

Triggered when the form submission specifies `product_review` as the `bc-action` parameter.

Processes product reviews submitted by customers and saves them to the catalog system.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`submission` | `array` | The sanitized form submission data containing customer review details such as rating and comments.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 209](BigCommerce/Container/Forms.php#L209-L217)

### `bigcommerce/form/action=Switch_Currency_Handler::ACTION`

Handles the currency switch action in the BigCommerce form submission.

This action is triggered when the user submits a form that includes a request to switch
the currency. The callback function handles the form submission and invokes the
`Switch_Currency_Handler` to process the currency change request.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`submission` | `array` | The form submission data, including the selected currency.
`container` | `\BigCommerce\Forms\Switch_Currency_Handler` | The container holding the `SWITCH_CURRENCY` handler.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 247](BigCommerce/Container/Forms.php#L247-L263)

### `bigcommerce/form/error`

Triggered when an error occurs during a form submission. Allows developers to handle or log form submission errors.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`error` | `\WP_Error` | The error object representing the validation or processing error. Contains error codes and messages.
`submission` | `array` | The sanitized form submission data (usually $_POST).
`redirect` | `string` | The URL to redirect the user after processing the error. Defaults to the home URL.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 271](BigCommerce/Container/Forms.php#L271-L280)

### `bigcommerce/form/success`

Handles form success and processes related actions.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`message` | `string` | The success message.
`submission` | `array` | The form submission data.
`url` | `string\|null` | Optional redirect URL.
`data` | `array` | Additional data associated with the submission.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 301](BigCommerce/Container/Forms.php#L301-L313)

### `bigcommerce/form/redirect`

Handles the form redirect action.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The redirect URL.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 321](BigCommerce/Container/Forms.php#L321-L330)

### `init`

Registers CLI commands during the `init` hook.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`` | `void` | 

Source: [src/BigCommerce/Container/Cli.php](BigCommerce/Container/Cli.php), [line 90](BigCommerce/Container/Cli.php#L90-L107)

### `bigcommerce/import/start`

Action to truncate the log when the BigCommerce import starts.

This action is triggered at the start of the BigCommerce import process. It clears or truncates the log file to ensure that old logs do not interfere with the new import process.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Log.php](BigCommerce/Container/Log.php), [line 89](BigCommerce/Container/Log.php#L89-L98)

### `bigcommerce/import/product/error`

Action to log product import errors.

This action is triggered when a product import encounters an error. It logs the error details including the product ID, catalog API, and the exception that caused the error.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`product_id` | `int` | The ID of the product being imported.
`catalog_api` | `\BigCommerce\Api\v3\Api\CatalogApi` | The catalog API instance used to fetch product data.
`exception` | `\Exception` | The exception that was thrown during the import.

Source: [src/BigCommerce/Container/Log.php](BigCommerce/Container/Log.php), [line 100](BigCommerce/Container/Log.php#L100-L112)

### `bigcommerce/log`

Action to log messages during the BigCommerce logging process.

This action is triggered when a log entry needs to be created. It logs the message, context, level, and path to the log file.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`level` | `string` | The log level (e.g., INFO, ERROR).
`message` | `string` | The log message to be recorded.
`context` | `array` | Additional context for the log entry.
`path` | `string` | The path where the log is being written.

Source: [src/BigCommerce/Container/Log.php](BigCommerce/Container/Log.php), [line 130](BigCommerce/Container/Log.php#L130-L141)

### `bigcommerce/import/log`

Action to log messages during the BigCommerce import process.

This action is triggered during the BigCommerce import process to log important messages. It captures the log level, message, context, and path for further troubleshooting.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`level` | `string` | The log level (e.g., INFO, ERROR).
`message` | `string` | The log message to be recorded.
`context` | `array` | Additional context for the log entry.

Source: [src/BigCommerce/Container/Log.php](BigCommerce/Container/Log.php), [line 143](BigCommerce/Container/Log.php#L143-L153)

### `bigcommerce/import/error`

Action to log import errors during the BigCommerce import process.

This action is triggered when there is an error during the import process. It logs the error message and context for further analysis.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`message` | `string` | The error message to be logged.
`context` | `array` | Additional context for the error.

Source: [src/BigCommerce/Container/Log.php](BigCommerce/Container/Log.php), [line 155](BigCommerce/Container/Log.php#L155-L166)

### `wp_kses_allowed_html`

Adds a callback to filter allowed HTML tags in KSES for product descriptions.

This action hooks into `wp_kses_allowed_html` to filter the allowed HTML tags
for product descriptions based on the provided context.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`allowed_tags` | `string\|array` | The allowed HTML tags.
`context` | `string` | The context for the allowed tags (e.g., 'post', 'comment', etc.).

Source: [src/BigCommerce/Container/Util.php](BigCommerce/Container/Util.php), [line 33](BigCommerce/Container/Util.php#L33-L54)

### `bigcommerce/create_account/submit_request`

Action to handle the submission of account creation requests.

This action processes data submitted for account creation, logs errors,
and invokes the Create_Account service to handle the request.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | Submitted data for account creation.
`errors` | `array` | An array of errors, if any, encountered during submission.

Source: [src/BigCommerce/Container/Merchant.php](BigCommerce/Container/Merchant.php), [line 119](BigCommerce/Container/Merchant.php#L119-L132)

### `admin_post_Connect_Account::CONNECT_ACTION`

Action to handle the account connection process.

Triggers the Connect_Account service to connect the merchant's account.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Merchant.php](BigCommerce/Container/Merchant.php), [line 158](BigCommerce/Container/Merchant.php#L158-L167)

### `bigcommerce/settings/after_content/page=Pending_Account_Screen::NAME`

Action to render the account status placeholder on settings pages.

Displays a placeholder for account status on specific admin settings pages.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Merchant.php](BigCommerce/Container/Merchant.php), [line 181](BigCommerce/Container/Merchant.php#L181-L190)

### `wp_ajax_Account_Status::STATUS_AJAX`

Action to handle AJAX requests for account status updates.

Handles requests to check and refresh the merchant's account status.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Merchant.php](BigCommerce/Container/Merchant.php), [line 192](BigCommerce/Container/Merchant.php#L192-L201)

### `bigcommerce/pending_account/check_status`

Action to handle status checks for pending accounts.

Processes errors during status checks and updates the account status as needed.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`errors` | `array` | An array of errors encountered during the status check.

Source: [src/BigCommerce/Container/Merchant.php](BigCommerce/Container/Merchant.php), [line 203](BigCommerce/Container/Merchant.php#L203-L213)

### `rest_api_init`

Registers the proxy controller routes when the REST API is initialized.

This action hooks into the `rest_api_init` action and ensures that the
proxy controller's routes are registered during the API initialization process.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The container instance.

Source: [src/BigCommerce/Container/Proxy.php](BigCommerce/Container/Proxy.php), [line 108](BigCommerce/Container/Proxy.php#L108-L124)

### `bigcommerce/proxy/response_received`

Action triggered when a response is received from the proxy.

This action hooks into the `bigcommerce/proxy/response_received` event and
handles the caching of the result after the response is received.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`result` | `mixed` | The response result from the proxy request.
`args` | `array` | The arguments passed to the proxy request.

Source: [src/BigCommerce/Container/Proxy.php](BigCommerce/Container/Proxy.php), [line 183](BigCommerce/Container/Proxy.php#L183-L206)

### `bigcommerce/webhooks/product_updated`

Action triggered when a product is updated.

This action hooks into the `bigcommerce/webhooks/product_updated` event and
handles clearing the cache for the updated product.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`product_id` | `array` | The updated product ID.

Source: [src/BigCommerce/Container/Proxy.php](BigCommerce/Container/Proxy.php), [line 208](BigCommerce/Container/Proxy.php#L208-L226)

### `rest_api_init`

Registers the AMP cart controller routes when the REST API is initialized.

This action hooks into the `rest_api_init` action and ensures that the
AMP cart controller's routes are registered during the API initialization process.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Proxy.php](BigCommerce/Container/Proxy.php), [line 248](BigCommerce/Container/Proxy.php#L248-L262)

### `media_buttons`

Renders the "Add Products" button in the media buttons section of the editor.

This action adds a custom button to the media buttons section in the WordPress admin
editor, which triggers the rendering of the products button when clicked.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`editor_id` | `string` | The ID of the editor instance.

Source: [src/BigCommerce/Container/Editor.php](BigCommerce/Container/Editor.php), [line 77](BigCommerce/Container/Editor.php#L77-L87)

### `enqueue_block_editor_assets`

Enqueues the dialog template assets for the block editor.

This action ensures that the dialog template is loaded when the block editor is used,
either by directly rendering it or by delaying the output until the appropriate time.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Editor.php](BigCommerce/Container/Editor.php), [line 101](BigCommerce/Container/Editor.php#L101-L127)

### `admin_enqueue_scripts`

Enqueues the dialog template assets for the block editor.

This action ensures that the dialog template is loaded when the block editor is used,
either by directly rendering it or by delaying the output until the appropriate time.
If Gutenberg is already enabled, the callback is triggered immediately, otherwise,
it is delayed until the `admin_enqueue_scripts` action is called.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Editor.php](BigCommerce/Container/Editor.php), [line 117](BigCommerce/Container/Editor.php#L117-L125)

### `admin_print_footer_scripts`

Prints the editor dialog template in the footer when the block editor is not enabled.

This action ensures that the dialog template is included in the footer when not using
the block editor, so that it can still be rendered for the classic editor.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Editor.php](BigCommerce/Container/Editor.php), [line 129](BigCommerce/Container/Editor.php#L129-L135)

### `init`

Registers the Gutenberg blocks for the block editor.

This action registers all the custom blocks related to BigCommerce that will be available
in the Gutenberg editor. It checks if the `register_block_type` function is available
before registering the blocks.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Editor.php](BigCommerce/Container/Editor.php), [line 183](BigCommerce/Container/Editor.php#L183-L198)

### `admin_head`

Enqueues customizer styles for the admin area.

This action ensures that customizer styles are applied to the admin area, affecting
how elements are displayed and styled within the backend of the WordPress site.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Editor.php](BigCommerce/Container/Editor.php), [line 231](BigCommerce/Container/Editor.php#L231-L239)

### `wp_head`

Outputs Segment analytics tracking code in the header. Injects the necessary JavaScript for Segment tracking on all pages.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Analytics.php](BigCommerce/Container/Analytics.php), [line 100](BigCommerce/Container/Analytics.php#L100-L103)

### `init`

Initializes the cron job processing for the import.

This action is hooked to the 'init' hook to ensure that cron jobs are processed during the init phase.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 265](BigCommerce/Container/Import.php#L265-L275)

### `init`

Fired on the 'init' action to schedule a queue processor task.

This hook schedules the queue processor if necessary, using the `$schedules` array.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`schedules` | `array` | The array of scheduled tasks.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 291](BigCommerce/Container/Import.php#L291-L302)

### `init`

Runs the lock expiration check during the init phase.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 304](BigCommerce/Container/Import.php#L304-L311)

### `update_option_Import_Settings::OPTION_FREQUENCY`

Updates the cron schedule when the import frequency setting is updated.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`old_value` | `string` | The old value of the cron schedule.
`new_value` | `string` | The new value of the cron schedule.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 313](BigCommerce/Container/Import.php#L313-L324)

### `bigcommerce/import/run`

Starts the import process when the `bigcommerce/import/run` action is triggered.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`status` | `string` | The status of the import process.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 326](BigCommerce/Container/Import.php#L326-L334)

### `Runner\Cron_Runner::START_CRON`

Begins the import process when the `Runner\Cron_Runner::START_CRON` action is triggered.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 336](BigCommerce/Container/Import.php#L336-L345)

### `Runner\Cron_Runner::CONTINUE_CRON`

Continues the import process when the `Runner\Cron_Runner::CONTINUE_CRON` action is triggered.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 347](BigCommerce/Container/Import.php#L347-L354)

### `Runner\AsyncProcessing_Runner::CONTINUE_IMPORT`

Executes the asynchronous import when the `Runner\AsyncProcessing_Runner::CONTINUE_IMPORT` action is triggered.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 356](BigCommerce/Container/Import.php#L356-L366)

### `Processors\Cleanup::CLEAN_USERS_TRANSIENT`

Cleans up customer group transients when the `Processors\Cleanup::CLEAN_USERS_TRANSIENT` action is triggered.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 368](BigCommerce/Container/Import.php#L368-L375)

### `Processors\Cleanup::PURGE_PRODUCTS`

Purges deleted products when the `Processors\Cleanup::PURGE_PRODUCTS` action is triggered.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 377](BigCommerce/Container/Import.php#L377-L384)

### `Processors\Cleanup::CLEAN_PRODUCTS_TRANSIENT`

Cleans product data transients when the `Processors\Cleanup::CLEAN_PRODUCTS_TRANSIENT` action is triggered.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`offset` | `int` | The offset for fetching data.
`partially` | `bool` | Whether to fetch partially or not.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 386](BigCommerce/Container/Import.php#L386-L395)

### `Manager::CRON_PROCESSOR`

Processes postponed tasks when the `Manager::CRON_PROCESSOR` action is triggered.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 397](BigCommerce/Container/Import.php#L397-L404)

### `bigcommerce/import/start`

Starts the import process when the `bigcommerce/import/start` action is triggered.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 519](BigCommerce/Container/Import.php#L519-L524)

### `bigcommerce/import/run`

Fired when the 'bigcommerce/import/run' action is triggered to process the next import task.

This hook attempts to run the next task in the import process and handles any exceptions by triggering error and log actions.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`status` | `string` | The status of the current import process.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 621](BigCommerce/Container/Import.php#L621-L635)

### `bigcommerce/import/error`

Fired when an error occurs during the BigCommerce import process.

This hook allows handling errors and custom logging or responses when an import error is encountered.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`error` | `string` | The error message from the import process.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 641](BigCommerce/Container/Import.php#L641-L648)

### `bigcommerce/import/before`

Fired before the BigCommerce import process begins. This hook is used to execute any necessary tasks before starting the import, such as cache flushing.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 659](BigCommerce/Container/Import.php#L659-L660)

### `bigcommerce/import/after`

Fired after the BigCommerce import process finishes. This hook is used to execute any necessary tasks after the import, such as cache flushing.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 662](BigCommerce/Container/Import.php#L662-L663)

### `admin_enqueue_scripts`

Enqueues admin scripts and styles.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Assets.php](BigCommerce/Container/Assets.php), [line 152](BigCommerce/Container/Assets.php#L152-L163)

### `admin_enqueue_scripts`

Removes Google Site Kit scripts on BigCommerce admin pages to prevent conflicts.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Assets.php](BigCommerce/Container/Assets.php), [line 165](BigCommerce/Container/Assets.php#L165-L176)

### `after_setup_theme`

Registers custom image sizes for the theme.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Assets.php](BigCommerce/Container/Assets.php), [line 213](BigCommerce/Container/Assets.php#L213-L221)

### `wp_enqueue_scripts`

Enqueues frontend scripts and styles.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`hook_suffix` | `string` | The current page's hook suffix.

Source: [src/BigCommerce/Container/Assets.php](BigCommerce/Container/Assets.php), [line 223](BigCommerce/Container/Assets.php#L223-L235)

### `init`

Register all taxonomy configurations during the 'init' action.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 190](BigCommerce/Container/Taxonomies.php#L190-L199)

### `pre_get_posts`

Apply Product Category filters to the query before fetching posts.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`query` | `\BigCommerce\Container\WP_Query` | The query object.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 229](BigCommerce/Container/Taxonomies.php#L229-L237)

### `parse_tax_query`

Hide child categories by default during tax query parsing.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`query` | `\BigCommerce\Container\WP_Tax_Query` | The tax query object.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 239](BigCommerce/Container/Taxonomies.php#L239-L245)

### `bigcommerce/import/start`

Fires when the BigCommerce import process starts.

This hook cancels any ongoing import process if necessary.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The container object.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 291](BigCommerce/Container/Taxonomies.php#L291-L299)

### `admin_notices`

Fires when an admin notice should be displayed.

This hook is used to trigger the admin notice for the channel synchronization status.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The container object.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 302](BigCommerce/Container/Taxonomies.php#L302-L310)

### `bigcommerce/settings/before_form/page=Connect_Channel_Screen::NAME`

This class is responsible for managing and registering taxonomies for BigCommerce integration. It defines constants for various taxonomies and handles their configuration and filtering via WordPress hooks.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 30](BigCommerce/Container/Taxonomies.php#L30-L318)

### `bigcommerce/import/start`

This class is responsible for managing and registering taxonomies for BigCommerce integration. It defines constants for various taxonomies and handles their configuration and filtering via WordPress hooks.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 30](BigCommerce/Container/Taxonomies.php#L30-L319)

### `bigcommerce/settings/before_form/page=Settings_Screen::NAME`

Registers a callback for initial channel sync before the form on the settings screen.

This action triggers a channel sync before the form is displayed in the settings.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The container object.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 321](BigCommerce/Container/Taxonomies.php#L321-L329)

### `edited_Channel\Channel::NAME`

Registers an action when the channel name is edited.

This hook triggers a function to handle channel name changes upon term edit.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`term_id` | `int` | The term ID of the edited channel.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 331](BigCommerce/Container/Taxonomies.php#L331-L339)

### `admin_menu`

Registers an action to create the first channel when the admin menu is loaded.

This action checks certain conditions and triggers the creation of the first channel.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The container object.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 346](BigCommerce/Container/Taxonomies.php#L346-L361)

### `load-edit.php`

Registers actions for filtering the product list table based on the selected channel.

This action filters the product list table on the admin page based on the selected channel.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The container object.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 398](BigCommerce/Container/Taxonomies.php#L398-L437)

### `pre_get_posts`

Filters the query by the selected channel before the posts are retrieved.

This action applies a filter to modify the query based on the selected channel.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`query` | `\BigCommerce\Container\WP_Query` | The query object.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 443](BigCommerce/Container/Taxonomies.php#L443-L453)

### `pre_option_BigCommerce\Settings\Sections\Currency::CURRENCY_CODE`

Filters the currency code before the option is retrieved.

This action applies a filter to modify the currency code based on the selected channel.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`currency_code` | `string` | The currency code to be filtered.
`container` | `\Pimple\Container` | The container object.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 459](BigCommerce/Container/Taxonomies.php#L459-L468)

### `bigcommerce/channel/updated_channel_id`

Sets routes for a specific channel when the channel ID is updated.

This action hooks into the `bigcommerce/channel/updated_channel_id` event and triggers the
`set_routes` method of the `Routes` class to update the routes for the specified channel.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`channel_id` | `int` | The ID of the updated channel.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 476](BigCommerce/Container/Taxonomies.php#L476-L488)

### `bigcommerce/routes/cron/update`

Updates routes via a cron job.

This action hooks into the `bigcommerce/routes/cron/update` event and triggers the
`update_routes` method of the `Routes` class to perform an update to the routes.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 490](BigCommerce/Container/Taxonomies.php#L490-L500)

### `update_option_show_on_front`

Schedules a route update when the `show_on_front` option is updated.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `show_on_front` option is updated.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 506](BigCommerce/Container/Taxonomies.php#L506-L513)

### `add_option_show_on_front`

Schedules a route update when the `show_on_front` option is added.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `show_on_front` option is added.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 515](BigCommerce/Container/Taxonomies.php#L515-L522)

### `update_option_permalink_structure`

Schedules a route update when the `permalink_structure` option is updated.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `permalink_structure` option is updated.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 524](BigCommerce/Container/Taxonomies.php#L524-L531)

### `add_option_permalink_structure`

Schedules a route update when the `permalink_structure` option is added.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `permalink_structure` option is added.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 533](BigCommerce/Container/Taxonomies.php#L533-L540)

### `update_option_Cart_Page::NAME`

Schedules a route update when the `Cart_Page` option is updated.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `Cart_Page` option is updated.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 542](BigCommerce/Container/Taxonomies.php#L542-L549)

### `add_option_Cart_Page::NAME`

Schedules a route update when the `Cart_Page` option is updated or added.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `Cart_Page` option is added.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 551](BigCommerce/Container/Taxonomies.php#L551-L558)

### `update_option_Login_Page::NAME`

Schedules a route update when the `Login_Page` option is updated.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `Login_Page` option is updated.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 560](BigCommerce/Container/Taxonomies.php#L560-L567)

### `add_option_Login_Page::NAME`

Schedules a route update when the `Login_Page` option is added.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `Login_Page` option is added.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 569](BigCommerce/Container/Taxonomies.php#L569-L576)

### `update_option_Account_Page::NAME`

Schedules a route update when the `Account_Page` option is updated.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `Account_Page` option is updated.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 578](BigCommerce/Container/Taxonomies.php#L578-L585)

### `add_option_Account_Page::NAME`

Schedules a route update when the `Account_Page` option is added.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `Account_Page` option is added.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 587](BigCommerce/Container/Taxonomies.php#L587-L594)

### `update_option_Shipping_Returns_Page::NAME`

Schedules a route update when the `Shipping_Returns_Page` option is updated.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `Shipping_Returns_Page` option is updated.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 596](BigCommerce/Container/Taxonomies.php#L596-L603)

### `add_option_Shipping_Returns_Page::NAME`

Schedules a route update when the `Shipping_Returns_Page` option is added.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `Shipping_Returns_Page` option is added.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 605](BigCommerce/Container/Taxonomies.php#L605-L612)

### `update_option_Product_Archive::ARCHIVE_SLUG`

Schedules a route update when the `Product_Archive::ARCHIVE_SLUG` option is updated.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `Product_Archive::ARCHIVE_SLUG` option is updated.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 614](BigCommerce/Container/Taxonomies.php#L614-L621)

### `add_option_Product_Archive::ARCHIVE_SLUG`

Schedules a route update when the `Product_Archive::ARCHIVE_SLUG` option is added.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `Product_Archive::ARCHIVE_SLUG` option is added.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 623](BigCommerce/Container/Taxonomies.php#L623-L630)

### `update_option_Product_Archive::CATEGORY_SLUG`

Schedules a route update when the `Product_Archive::CATEGORY_SLUG` option is updated.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `Product_Archive::CATEGORY_SLUG` option is updated.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 632](BigCommerce/Container/Taxonomies.php#L632-L639)

### `add_option_Product_Archive::CATEGORY_SLUG`

Schedules a route update when the `Product_Archive::CATEGORY_SLUG` option is added.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `Product_Archive::CATEGORY_SLUG` option is added.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 641](BigCommerce/Container/Taxonomies.php#L641-L648)

### `update_option_Product_Archive::BRAND_SLUG`

Schedules a route update when the `Product_Archive::BRAND_SLUG` option is updated.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `Product_Archive::BRAND_SLUG` option is updated.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 650](BigCommerce/Container/Taxonomies.php#L650-L657)

### `add_option_Product_Archive::BRAND_SLUG`

Schedules a route update when the `Product_Archive::BRAND_SLUG` option is added.

Triggers the `schedule_update_routes` method of the `Routes` class whenever the `Product_Archive::BRAND_SLUG` option is added.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 659](BigCommerce/Container/Taxonomies.php#L659-L666)

### `bigcommerce/channel/connection_changed`

Schedules a route update when the channel connection changes.

Triggers the `schedule_update_routes` method in the `Routes` class to ensure routes are updated
when the channel connection status changes.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 668](BigCommerce/Container/Taxonomies.php#L668-L676)

### `update_option_home`

Updates site home route when the site's home option is updated.

Triggers the `update_site_home` method of the `Routes` class to refresh the site home route when the `home` option is changed.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 678](BigCommerce/Container/Taxonomies.php#L678-L687)

### `post_updated`

Updates the route's permalink when a post is updated.

Checks if a route is associated with
the post and triggering the `update_route_permalink` method of the `Routes` class to update
the permalink if needed.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_id` | `int` | The ID of the updated post.
`new_post` | `object` | The new post object after the update.
`old_post` | `object` | The old post object before the update.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 689](BigCommerce/Container/Taxonomies.php#L689-L704)

### `bigcommerce/import/fetched_store_settings`

Checks and updates routes after fetching store settings during an import.

Triggers the `maybe_update_routes` method of the `Routes` class to ensure routes are updated
after store settings are fetched during the import process.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 706](BigCommerce/Container/Taxonomies.php#L706-L716)

### `rest_api_init`

Initializes REST API routes during the 'rest_api_init' action.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 371](BigCommerce/Container/Rest.php#L371-L384)

### `bigcommerce/action_endpoint/Amp_Cart::CHECKOUT_REDIRECT_ACTION`

This action is triggered when the AMP checkout redirect endpoint is accessed.

The callback handles the redirection request using the AMP Cart instance.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`args` | `array` | Arguments passed to the action.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 151](BigCommerce/Container/Amp.php#L151-L165)

### `wp`

Initializes AMP template overrides based on the current request context.

This action determines if AMP template overrides should be enabled, typically
for rendering plugin templates in AMP-compatible mode. When enabled, it applies
various filters to modify template paths, data, and behaviors specific to AMP.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`wp` | `\BigCommerce\Container\WP` | The WordPress environment object passed to the 'wp' action. Provides access to query variables and the request context.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 171](BigCommerce/Container/Amp.php#L171-L387)

### `bigcommerce/form/before_redirect`

Action to modify AMP redirect headers before form submission.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The URL being redirected to.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 389](BigCommerce/Container/Amp.php#L389-L396)

### `amp_post_template_css`

Action to output custom AMP CSS for a post template.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 398](BigCommerce/Container/Amp.php#L398-L402)

### `amp_post_template_head`

Action to output AMP-specific scripts in the `<head>` section.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 418](BigCommerce/Container/Amp.php#L418-L421)

### `after_setup_theme`

Action to register AMP-specific menus after theme setup.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 423](BigCommerce/Container/Amp.php#L423-L428)

### `admin_notices`

Action to display AMP admin notices in the WordPress admin.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 444](BigCommerce/Container/Amp.php#L444-L450)

### `setup_theme`

Hooks into 'setup_theme' to load compatibility functions for WooCommerce.

This action is triggered during theme setup to ensure compatibility with WooCommerce
when activating or updating the plugin.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Compatibility.php](BigCommerce/Container/Compatibility.php), [line 106](BigCommerce/Container/Compatibility.php#L106-L121)

### `wp`

Hooks into 'wp' to fix Flatsome theme compatibility for the account page.

This action is triggered when WordPress initializes the current page to ensure
that the Flatsome theme's content fix is removed for the account page.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Compatibility.php](BigCommerce/Container/Compatibility.php), [line 123](BigCommerce/Container/Compatibility.php#L123-L135)

### `init`

Hooks into 'init' to disable WooCommerce shortcodes in Flatsome theme.

This action is triggered during the initialization of WordPress to replace
WooCommerce-related shortcodes with a null return for compatibility with the Flatsome theme.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Compatibility.php](BigCommerce/Container/Compatibility.php), [line 137](BigCommerce/Container/Compatibility.php#L137-L156)

### `init`

Hooks into 'init' to load compatibility functions for WordPress 4.9.

This action checks if the current WordPress version is below 4.9 and includes
compatibility functions specific to that version.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Compatibility.php](BigCommerce/Container/Compatibility.php), [line 158](BigCommerce/Container/Compatibility.php#L158-L170)

### `init`

Hooks into 'init' to load compatibility functions for WordPress 5.1.

This action checks if the current WordPress version is below 5.1 and includes
compatibility functions specific to that version.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Compatibility.php](BigCommerce/Container/Compatibility.php), [line 172](BigCommerce/Container/Compatibility.php#L172-L184)

### `pre_option_woocommerce_myaccount_page_id`

Filters the My Account page ID for WooCommerce.

This action is triggered when retrieving the 'woocommerce_myaccount_page_id' option.
It ensures that the correct page ID is used for logged-in users.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Compatibility.php](BigCommerce/Container/Compatibility.php), [line 186](BigCommerce/Container/Compatibility.php#L186-L199)

### `admin_notices`

Displays an admin notice to verify checkout requirements if the setup status meets the requirements.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Checkout.php](BigCommerce/Container/Checkout.php), [line 57](BigCommerce/Container/Checkout.php#L57-L62)

### `admin_post_Requirements_Notice::REFRESH`

Refreshes the checkout requirements status by calling the `refresh_status` method.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Checkout.php](BigCommerce/Container/Checkout.php), [line 64](BigCommerce/Container/Checkout.php#L64-L67)

### `load-nav-menus.php`

Adds a metabox for navigation items.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Nav_Menu.php](BigCommerce/Container/Nav_Menu.php), [line 93](BigCommerce/Container/Nav_Menu.php#L93-L100)

### `wp_ajax_add-menu-item`

Handles AJAX requests to add menu items.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Nav_Menu.php](BigCommerce/Container/Nav_Menu.php), [line 102](BigCommerce/Container/Nav_Menu.php#L102-L109)

### `added_post_meta`

Registers review-related services in the container.

Services include:
- Product update listener for tracking metadata changes.
- Review fetcher for retrieving reviews from the API.
- Review cache for caching reviews and updating the cache on product updates.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The DI container for registering services.

Source: [src/BigCommerce/Container/Reviews.php](BigCommerce/Container/Reviews.php), [line 39](BigCommerce/Container/Reviews.php#L39-L74)

### `updated_post_meta`

Registers review-related services in the container.

Services include:
- Product update listener for tracking metadata changes.
- Review fetcher for retrieving reviews from the API.
- Review cache for caching reviews and updating the cache on product updates.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The DI container for registering services.

Source: [src/BigCommerce/Container/Reviews.php](BigCommerce/Container/Reviews.php), [line 39](BigCommerce/Container/Reviews.php#L39-L75)

### `Product_Update_Listener::TRIGGER_UPDATE`

Callback for updating the review cache.

Triggered when a product update event occurs.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`product_id` | `int` | The ID of the updated product.

Source: [src/BigCommerce/Container/Reviews.php](BigCommerce/Container/Reviews.php), [line 99](BigCommerce/Container/Reviews.php#L99-L108)

## Filters

### `bigcommerce/customer/create/args`

Filters the arguments used to create a customer in BigCommerce.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | The customer creation arguments.

Source: [src/BigCommerce/Forms/Registration_Handler.php](BigCommerce/Forms/Registration_Handler.php), [line 136](BigCommerce/Forms/Registration_Handler.php#L136-L141)

### `bigcommerce/currency/code`

Filter the currency code used for cart operations.

This filter temporarily overrides the currency code to use the new currency
during the cart recreation process.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`new_currency_code` | `string` | The currency code to use.

Source: [src/BigCommerce/Forms/Switch_Currency_Handler.php](BigCommerce/Forms/Switch_Currency_Handler.php), [line 181](BigCommerce/Forms/Switch_Currency_Handler.php#L181-L189)

### `bigcommerce/cart/cart_id`

Filter the cart ID used for cart operations.

This filter temporarily overrides the cart ID to use the value from the COOKIE
global during the cart recreation process.

**Arguments**

No arguments.

Source: [src/BigCommerce/Forms/Switch_Currency_Handler.php](BigCommerce/Forms/Switch_Currency_Handler.php), [line 196](BigCommerce/Forms/Switch_Currency_Handler.php#L196-L204)

### `bigcommerce/button/purchase`

Filter to overwrite the purchase button HTML.

Temporarily modifies the button in the product form preview to be disabled.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`html` | `string` | The original button HTML.
`post_id` | `int` | The product post ID.
`label` | `string` | The label for the button.

Source: [src/BigCommerce/Templates/Product_Form_Preview.php](BigCommerce/Templates/Product_Form_Preview.php), [line 46](BigCommerce/Templates/Product_Form_Preview.php#L46-L57)

### `pre_term_description`

Filters the term description before it is saved or displayed.

This hook is used to apply content sanitization to term descriptions.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`description` | `string` | The term description before filtering.

Source: [src/BigCommerce/Import/Processors/Term_Import.php](BigCommerce/Import/Processors/Term_Import.php), [line 159](BigCommerce/Import/Processors/Term_Import.php#L159-L167)

### `bigcommerce/template=components/catalog/product-archive.php/data`

Remove the refinery component from the product archive template.

This method filters the product archive template data to remove the refinery
component, which may be used for facets or filtering options in the catalog.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`template_data` | `array` | The template data array, which is modified to remove the refinery component.

Source: [src/BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.php](BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.php), [line 83](BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.php#L83-L92)

### `bigcommerce/template=components/catalog/product-archive.php/data`

Customize the page title for the product archive based on wishlist information.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`template_data` | `array` | The template data array, which is modified to include the wishlist name as the page title.

Source: [src/BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.php](BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.php), [line 94](BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.php#L94-L100)

### `post_type_archive_title`

Customize the WordPress archive title for wishlist pages.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`title` | `string` | The current archive title.
`post_type` | `string` | The post type for which the archive is being displayed.

Source: [src/BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.php](BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.php), [line 102](BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.php#L102-L109)

### `bigcommerce/template=components/catalog/no-results.php/data`

Customize the "No Results" message for wishlist-related templates.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`template_data` | `array` | The template data array, modified to include wishlist-specific "No Results" messages and labels.

Source: [src/BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.php](BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.php), [line 111](BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.php#L111-L117)

### `rest_prepare_{$post->post_type}`

Filters the REST response for a post type, modifying the content if needed.

This filter is triggered when preparing a REST response for a post. It ensures
that any post content is processed before being returned to the API response.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`response` | `\WP_REST_Response` | The response object.
`post` | `\WP_Post` | Post object.
`request` | `\WP_REST_Request` | Request object.

**Changelog**

Version | Description
------- | -----------
`4.7.0` | 

Source: [src/BigCommerce/Editor/Gutenberg/Migrate_Blocks.php](BigCommerce/Editor/Gutenberg/Migrate_Blocks.php), [line 81](BigCommerce/Editor/Gutenberg/Migrate_Blocks.php#L81-L96)

### `the_editor_content`

Filters the content of the editor when using the classic editor.

This filter checks if the content matches the original post content. If it does,
it will attempt to replace blocks with shortcodes. If the content doesn't match
the original post content, it returns the unchanged content to avoid unnecessary
modification.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`content` | `string` | The content of the editor.
`default_editor` | `string` | The default editor being used.

Source: [src/BigCommerce/Editor/Gutenberg/Migrate_Blocks.php](BigCommerce/Editor/Gutenberg/Migrate_Blocks.php), [line 101](BigCommerce/Editor/Gutenberg/Migrate_Blocks.php#L101-L129)

### `bigcommerce/channel/listing/should_update`

Filter: Prevents product listings from being updated during import.

Temporarily disables updates to product listings to avoid conflicts.

**Arguments**

No arguments.

Source: [src/BigCommerce/Webhooks/Product/Product_Creator.php](BigCommerce/Webhooks/Product/Product_Creator.php), [line 75](BigCommerce/Webhooks/Product/Product_Creator.php#L75-L82)

### `bigcommerce/channel/listing/should_delete`

Filter: Prevents product listings from being deleted during import.

Temporarily disables deletion of product listings to preserve integrity.

**Arguments**

No arguments.

Source: [src/BigCommerce/Webhooks/Product/Product_Creator.php](BigCommerce/Webhooks/Product/Product_Creator.php), [line 84](BigCommerce/Webhooks/Product/Product_Creator.php#L84-L91)

### `bigcommerce/channel/listing/should_update`

Prevents product listing updates during the product re-import process.

This filter ensures that listing data for products is not automatically
updated when a product is being re-imported, maintaining the integrity of the
existing listings during the operation.

**Arguments**

No arguments.

Source: [src/BigCommerce/Webhooks/Product/Product_Updater.php](BigCommerce/Webhooks/Product/Product_Updater.php), [line 85](BigCommerce/Webhooks/Product/Product_Updater.php#L85-L92)

### `bigcommerce/channel/listing/should_delete`

Prevents product listing deletions during the product re-import process.

This filter ensures that listing data for products is not automatically
deleted when a product is being re-imported, preserving existing listings
until the process is complete.

**Arguments**

No arguments.

Source: [src/BigCommerce/Webhooks/Product/Product_Updater.php](BigCommerce/Webhooks/Product/Product_Updater.php), [line 94](BigCommerce/Webhooks/Product/Product_Updater.php#L94-L101)

### `bigcommerce/import/strategy/needs_refresh`

Filter to determine if products need to be refreshed.

This filter is applied when the 'force' flag is passed in the command arguments, forcing a refresh of all products.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`needs_refresh` | `bool` | Whether products need to be refreshed.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 70](BigCommerce/CLI/Import_Products.php#L70-L78)

### `bigcommerce/import/strategy/term/needs_refresh`

Filter to determine if terms need to be refreshed.

This filter is applied when the 'force' flag is passed in the command arguments, forcing a refresh of terms.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`needs_refresh` | `bool` | Whether terms need to be refreshed.

Source: [src/BigCommerce/CLI/Import_Products.php](BigCommerce/CLI/Import_Products.php), [line 80](BigCommerce/CLI/Import_Products.php#L80-L88)

### `bigcommerce/channel/listing/title`

Filters the listing title, providing an empty value during reset.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`value` | `string` | The listing title.

Source: [src/BigCommerce/Post_Types/Product/Reset_Listing.php](BigCommerce/Post_Types/Product/Reset_Listing.php), [line 133](BigCommerce/Post_Types/Product/Reset_Listing.php#L133-L140)

### `bigcommerce/channel/listing/description`

Filters the listing description, providing an empty value during reset.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`value` | `string` | The listing description.

Source: [src/BigCommerce/Post_Types/Product/Reset_Listing.php](BigCommerce/Post_Types/Product/Reset_Listing.php), [line 142](BigCommerce/Post_Types/Product/Reset_Listing.php#L142-L149)

### `posts_orderby`

Customize the SQL `ORDER BY` clause for posts.

This filter modifies the `ORDER BY` clause used in the SQL query for fetching posts,
enabling custom sorting logic.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`orderby` | `string` | The existing SQL `ORDER BY` clause.
`query` | `\BigCommerce\Post_Types\Product\WP_Query` | The current WP_Query instance.

Source: [src/BigCommerce/Post_Types/Product/Query.php](BigCommerce/Post_Types/Product/Query.php), [line 171](BigCommerce/Post_Types/Product/Query.php#L171-L182)

### `allowed_redirect_hosts`

Filters the allowed redirect hosts to include the checkout host from BigCommerce.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`hosts` | `array` | The array of allowed redirect hosts.

Source: [src/BigCommerce/Amp/Amp_Cart.php](BigCommerce/Amp/Amp_Cart.php), [line 137](BigCommerce/Amp/Amp_Cart.php#L137-L151)

### `bigcommerce/plugin/credentials_set`

Filters whether the API credentials are set.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`set` | `bool` | Whether the API credentials are set.

Source: [src/BigCommerce/Container/Api.php](BigCommerce/Container/Api.php), [line 211](BigCommerce/Container/Api.php#L211-L219)

### `bigcommerce/api/default_headers`

Filters the default headers for API requests.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`headers` | `array` | The default headers.

Source: [src/BigCommerce/Container/Api.php](BigCommerce/Container/Api.php), [line 221](BigCommerce/Container/Api.php#L221-L229)

### `bigcommerce/diagnostics`

Adds diagnostic data for webhook statuses.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | The existing diagnostic data.

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 380](BigCommerce/Container/Webhooks.php#L380-L389)

### `the_content`

Adds the gift certificates sub-navigation above the content.

This callback function is hooked into the `the_content` filter to insert the gift
certificates sub-navigation at the beginning of the content.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`content` | `string` | The post content.

Source: [src/BigCommerce/Container/Gift_Certificates.php](BigCommerce/Container/Gift_Certificates.php), [line 43](BigCommerce/Container/Gift_Certificates.php#L43-L55)

### `wp_setup_nav_menu_item`

Filters the navigation menu item to add classes for the cart page.

This filter is applied when setting up the navigation menu item to ensure that
the appropriate classes are added to the cart page menu item.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`menu_item` | `\WP_Post` | The menu item object to be filtered.

Source: [src/BigCommerce/Container/Cart.php](BigCommerce/Container/Cart.php), [line 159](BigCommerce/Container/Cart.php#L159-L171)

### `bigcommerce/js_config`

Filters the JavaScript configuration for the mini cart.

This filter modifies the `js_config` array to include specific configurations
related to the mini cart, such as display options and functionality.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`config` | `array` | The existing JavaScript configuration.

Source: [src/BigCommerce/Container/Cart.php](BigCommerce/Container/Cart.php), [line 268](BigCommerce/Container/Cart.php#L268-L280)

### `bigcommerce/settings/settings_url`

Filters the settings URL for the settings screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | Current settings URL.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 365](BigCommerce/Container/Settings.php#L365-L372)

### `pre_option_Api_Credentials::OPTION_STORE_URL`

Applies environment overrides for API credential options.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`value` | `mixed` | Current value of the option.
`option` | `string` | Name of the option.
`default` | `mixed` | Default value of the option.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 475](BigCommerce/Container/Settings.php#L475-L484)

### `pre_option_Api_Credentials::OPTION_CLIENT_ID`

Filters the option value for API credentials client ID.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`value` | `mixed` | The option value.
`option` | `string` | The option name.
`default` | `mixed` | The default value to return if the option does not exist.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 486](BigCommerce/Container/Settings.php#L486-L494)

### `pre_option_Api_Credentials::OPTION_CLIENT_SECRET`

Filters the option value for API credentials client ID.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`value` | `mixed` | The option value.
`option` | `string` | The option name.
`default` | `mixed` | The default value to return if the option does not exist.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 496](BigCommerce/Container/Settings.php#L496-L504)

### `pre_option_Api_Credentials::OPTION_ACCESS_TOKEN`

Filters the option value for API credentials client ID.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`value` | `mixed` | The option value.
`option` | `string` | The option name.
`default` | `mixed` | The default value to return if the option does not exist.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 506](BigCommerce/Container/Settings.php#L506-L514)

### `pre_update_option_Api_Credentials::OPTION_STORE_URL`

Filters the value before an API credential option is updated.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`value` | `mixed` | The new option value.
`option` | `string` | The option name.
`old_value` | `mixed` | The old option value.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 550](BigCommerce/Container/Settings.php#L550-L558)

### `pre_update_option_Api_Credentials::OPTION_CLIENT_ID`

Filters the value before an API credential option is updated.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`value` | `mixed` | The new option value.
`option` | `string` | The option name.
`old_value` | `mixed` | The old option value.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 560](BigCommerce/Container/Settings.php#L560-L568)

### `pre_update_option_Api_Credentials::OPTION_CLIENT_SECRET`

Filters the value before an API credential option is updated.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`value` | `mixed` | The new option value.
`option` | `string` | The option name.
`old_value` | `mixed` | The old option value.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 570](BigCommerce/Container/Settings.php#L570-L578)

### `pre_update_option_Api_Credentials::OPTION_ACCESS_TOKEN`

Filters the value before an API credential option is updated.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`value` | `mixed` | The new option value.
`option` | `string` | The option name.
`old_value` | `mixed` | The old option value.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 580](BigCommerce/Container/Settings.php#L580-L588)

### `views_edit-Product::NAME`

Modifies the product list table view to include an import link if the configuration status
meets the required condition.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`views` | `array` | The views for the product list table.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 734](BigCommerce/Container/Settings.php#L734-L747)

### `bigcommerce/onboarding/error_redirect`

Filters the redirect URL during the onboarding error process.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The default URL to redirect to.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 998](BigCommerce/Container/Settings.php#L998-L1004)

### `bigcommerce/onboarding/reset`

Filters the URL to reset onboarding progress.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The default URL for resetting onboarding.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1005](BigCommerce/Container/Settings.php#L1005-L1011)

### `bigcommerce/settings/create_account_url`

Filters the URL for creating a BigCommerce account.

This filter allows modification of the URL used to create a BigCommerce account
during the onboarding process.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The current URL for the create account page.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1026](BigCommerce/Container/Settings.php#L1026-L1037)

### `bigcommerce/onboarding/success_redirect`

Filter to redirect the user after a successful onboarding.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The URL to redirect to after success.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1193](BigCommerce/Container/Settings.php#L1193-L1199)

### `bigcommerce/settings/credentials_url`

Provides various screens and settings for BigCommerce.

This class is responsible for registering settings screens, handling API credentials,
and managing various onboarding steps in the BigCommerce plugin.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 51](BigCommerce/Container/Settings.php#L51-L1224)

### `bigcommerce/settings/resources_url`

Filters the resources URL for the settings screen.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 1522](BigCommerce/Container/Settings.php#L1522-L1525)

### `request`

Filter triggered to modify the request variables before the query is processed.

This filter applies the `request` filter to modify the request variables by filtering
empty query vars using the `filter_empty_query_vars` method of the `PRODUCT_QUERY` container instance.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`vars` | `array` | The request variables to be filtered.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 199](BigCommerce/Container/Post_Types.php#L199-L211)

### `query_vars`

Filter triggered to add custom query variables.

This filter applies the `query_vars` filter to add additional query variables using
the `add_query_vars` method of the `PRODUCT_QUERY` container instance.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`vars` | `array` | The existing query variables.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 213](BigCommerce/Container/Post_Types.php#L213-L225)

### `wp_insert_post_data`

Filter triggered before inserting post data to prevent changes to the post slug.

This filter applies the `wp_insert_post_data` filter to prevent changes to the product's
slug during post insert or update using the `prevent_slug_changes` method of the `PRODUCT_ADMIN` container instance.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | The post data to be inserted or updated.
`submitted` | `array` | The submitted data from the post form.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 271](BigCommerce/Container/Post_Types.php#L271-L284)

### `get_sample_permalink_html`

Filter triggered to modify the sample permalink HTML for a post.

This filter applies the `get_sample_permalink_html` filter to override the HTML for the
sample permalink using the `override_sample_permalink_html` method of the `PRODUCT_ADMIN` container instance.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`html` | `string` | The HTML for the sample permalink.
`post_id` | `int` | The ID of the post.
`title` | `string` | The title of the post.
`slug` | `string` | The slug of the post.
`post` | `\WP_Post` | The post object.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 286](BigCommerce/Container/Post_Types.php#L286-L302)

### `pre_handle_404`

Filter triggered to handle product out-of-stock behavior and redirect if necessary.

This filter applies the `pre_handle_404` filter and checks if the queried product is out of stock. If the product
has a defined redirect URL, the user is redirected. Otherwise, the default 404 behavior is triggered.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`preempt` | `string` | The current preempted status of the 404 response.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 360](BigCommerce/Container/Post_Types.php#L360-L385)

### `views_edit-Product\Product::NAME`

Filter triggered to modify the product list table views for import status.

This filter adds or modifies views related to product import status in the admin list table for products.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`views` | `array` | The current set of views for the product list table.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 387](BigCommerce/Container/Post_Types.php#L387-L398)

### `views_edit-Product\Product::NAME`

Filter triggered to modify the product list table views for import tooltip.

This filter adds a tooltip to the product import status in the product list table in the admin interface.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`views` | `array` | The current set of views for the product list table.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 400](BigCommerce/Container/Post_Types.php#L400-L411)

### `views_edit-Product\Product::NAME`

Filter triggered to modify the product list table views for the manage link.

This filter modifies the views in the product list table by adding or modifying the manage link.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`views` | `array` | The current set of views for the product list table.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 413](BigCommerce/Container/Post_Types.php#L413-L424)

### `map_meta_cap`

Filter triggered to modify the meta capabilities for product post types.

This filter applies the `map_meta_cap` filter to disallow publication capabilities for the product post type.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`caps` | `array` | The current capabilities for the user.
`cap` | `string` | The capability being checked.
`user_id` | `int` | The ID of the user being checked.
`args` | `array` | Additional arguments.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 437](BigCommerce/Container/Post_Types.php#L437-L451)

### `display_post_states`

Filter triggered to modify the post states for unsupported products.

This filter is used to show an unsupported status for certain products in the WordPress admin.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_states` | `array` | The current post states.
`post` | `\WP_Post` | The post object.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 453](BigCommerce/Container/Post_Types.php#L453-L465)

### `wp_insert_post_data`

Filter triggered to prevent the publication of certain product posts.

This filter prevents the publication of certain products by modifying the post data using the `prevent_publication` method.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | The post data.
`postarr` | `array` | The post array.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 467](BigCommerce/Container/Post_Types.php#L467-L479)

### `bigcommerce/channel/listing/should_update`

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 504](BigCommerce/Container/Post_Types.php#L504-L504)

### `bigcommerce/channel/listing/should_delete`

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 505](BigCommerce/Container/Post_Types.php#L505-L505)

### `manage_bigcommerce_product_posts_columns`

Filter triggered to modify the columns in the BigCommerce product list table.

This filter is used to add additional columns, such as the BigCommerce product ID, to the product list table in the admin.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`columns` | `array` | The current list of columns.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 520](BigCommerce/Container/Post_Types.php#L520-L531)

### `bigcommerce/diagnostics`

Adds diagnostic data related to the sync log.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | Diagnostic data to be included in the output.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 635](BigCommerce/Container/Post_Types.php#L635-L646)

### `post_row_actions`

Adds a row action for the product post actions in the admin.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`actions` | `array` | The current actions for the post.
`post` | `\BigCommerce\Container\WP_Post` | The post object being displayed.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 661](BigCommerce/Container/Post_Types.php#L661-L673)

### `post_submitbox_misc_actions`

Adds a link to the submit box on the product post edit screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post` | `\BigCommerce\Container\WP_Post` | The post object being edited.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 675](BigCommerce/Container/Post_Types.php#L675-L686)

### `bigcommerce/gutenberg/js_config`

Adds a store link to the Gutenberg block editor configuration.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | The existing Gutenberg block editor configuration data.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 688](BigCommerce/Container/Post_Types.php#L688-L699)

### `post_row_actions`

Adds a reset action to the post row actions for product listings.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`actions` | `array` | The current actions for the post.
`post` | `\BigCommerce\Container\WP_Post` | The post object being displayed.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 727](BigCommerce/Container/Post_Types.php#L727-L739)

### `post_row_actions`

Adds a resync action to post row actions.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`actions` | `array` | The list of actions for the post.
`post` | `\BigCommerce\Container\WP_Post` | The post object.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 765](BigCommerce/Container/Post_Types.php#L765-L775)

### `bigcommerce/gutenberg/js_config`

Adds a channel indicator to the Gutenberg JS config.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | The Gutenberg JS config data.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 812](BigCommerce/Container/Post_Types.php#L812-L825)

### `wp_unique_post_slug`

Filters the unique post slug per channel.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`slug` | `string` | The current post slug.
`post_id` | `int` | The post ID.
`post_status` | `string` | The post status.
`post_type` | `string` | The post type.
`post_parent` | `int` | The parent post ID.
`original_slug` | `string` | The original slug.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 876](BigCommerce/Container/Post_Types.php#L876-L894)

### `wp_title_parts`

Modifies the WordPress title parts for products.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`title_parts` | `array` | The parts of the title.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 909](BigCommerce/Container/Post_Types.php#L909-L920)

### `document_title_parts`

Filters the product document title parts.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`title_parts` | `array` | The document title parts.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 922](BigCommerce/Container/Post_Types.php#L922-L931)

### `wp_head`

Filters the product page meta description.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Post_Types.php](BigCommerce/Container/Post_Types.php), [line 933](BigCommerce/Container/Post_Types.php#L933-L944)

### `login_url`

Filter login URL for custom redirection.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The login URL.
`redirect` | `string` | The URL to redirect to after login.
`reauth` | `bool` | Whether the login is a re-authentication attempt.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 226](BigCommerce/Container/Accounts.php#L226-L236)

### `wp_login_errors`

Filter login errors to handle custom error messages.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`errors` | `\WP_Error` | The login errors.
`redirect` | `string` | The URL to redirect to after login.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 238](BigCommerce/Container/Accounts.php#L238-L247)

### `lostpassword_url`

Filter lost password URL for custom redirection.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The lost password URL.
`redirect` | `string` | The URL to redirect to after password reset.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 249](BigCommerce/Container/Accounts.php#L249-L258)

### `lostpassword_user_data`

Filter user data before sending the lost password email.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`user_data` | `array` | User data.
`errors` | `\WP_Error` | Any errors found.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 260](BigCommerce/Container/Accounts.php#L260-L269)

### `register_url`

Filter registration URL for custom redirection.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The registration URL.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 280](BigCommerce/Container/Accounts.php#L280-L288)

### `authenticate`

Filter authentication process for new user login.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`user` | `\BigCommerce\Container\WP_User\|null` | The WP_User object on successful authentication, or null if authentication fails.
`username` | `string` | The username.
`password` | `string` | The password.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 298](BigCommerce/Container/Accounts.php#L298-L312)

### `check_password`

Filter password check for linked accounts.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`match` | `bool` | Whether the password matches.
`password` | `string` | The password to check.
`hash` | `string` | The stored password hash.
`user_id` | `int` | The user ID.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 314](BigCommerce/Container/Accounts.php#L314-L329)

### `bigcommerce/countries/data`

Adding filters to fetch and handle country data

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 366](BigCommerce/Container/Accounts.php#L366-L369)

### `bigcommerce/js_config`

Filter to modify the JavaScript configuration for BigCommerce's storefront.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`config` | `array` | The existing JavaScript configuration.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 375](BigCommerce/Container/Accounts.php#L375-L381)

### `bigcommerce/admin/js_config`

Filter to modify the JavaScript configuration for BigCommerce's admin panel.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`config` | `array` | The existing JavaScript configuration.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 383](BigCommerce/Container/Accounts.php#L383-L389)

### `wp_setup_nav_menu_item`

Action to filter account menu items

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 403](BigCommerce/Container/Accounts.php#L403-L406)

### `the_content`

Action to add subnav above content

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 413](BigCommerce/Container/Accounts.php#L413-L416)

### `bigcommerce/customer/group_info`

Filter to set customer group information

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 465](BigCommerce/Container/Accounts.php#L465-L468)

### `bigcommerce/forms/show_messages`

Filters the display of form messages.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`show` | `bool` | Whether to show messages.
`post_id` | `int` | The post ID.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 219](BigCommerce/Container/Forms.php#L219-L229)

### `bigcommerce/product/reviews/show_form`

Toggles the review form availability.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`enabled` | `bool` | Whether the review form is enabled.
`post_id` | `int` | The post ID.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 231](BigCommerce/Container/Forms.php#L231-L241)

### `bigcommerce/form/state/errors`

Filters the error data for the form state.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | Error data.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 282](BigCommerce/Container/Forms.php#L282-L293)

### `the_content`

Filters the content to render messages above the main content.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`content` | `string` | The post content.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 338](BigCommerce/Container/Forms.php#L338-L347)

### `bigcommerce/forms/messages`

Filters and renders the messages in the form.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`messages` | `array` | The form messages.

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 349](BigCommerce/Container/Forms.php#L349-L360)

### `bigcommerce/diagnostics`

Filter to add the log to the diagnostics output.

This filter is used to add the debug log to the BigCommerce diagnostics, providing valuable information for troubleshooting.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`diagnostics` | `array` | The array containing diagnostic information.

Source: [src/BigCommerce/Container/Log.php](BigCommerce/Container/Log.php), [line 114](BigCommerce/Container/Log.php#L114-L124)

### `bigcommerce/settings/connect_account_url`

Filter to modify the account connection URL.

Allows customization of the URL used to connect a BigCommerce account.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The default account connection URL.

Source: [src/BigCommerce/Container/Merchant.php](BigCommerce/Container/Merchant.php), [line 146](BigCommerce/Container/Merchant.php#L146-L156)

### `bigcommerce/proxy/result_pre`

Filters the proxy result before fetching from the cache.

This filter applies the `bigcommerce/proxy/result_pre` filter to modify or
cache the result before it is returned from the proxy. It allows for caching
the result before the response is sent back.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`result` | `mixed` | The result to be cached.
`args` | `array` | Arguments for the cache request.

Source: [src/BigCommerce/Container/Proxy.php](BigCommerce/Container/Proxy.php), [line 154](BigCommerce/Container/Proxy.php#L154-L181)

### `bigcommerce/admin/js_config`

Filters the JavaScript configuration for the admin editor dialog.

This filter allows modification of the JavaScript configuration for the dialog template
based on the provided settings, including necessary data for handling the products and
shortcode configurations.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`config` | `array` | The current JavaScript configuration for the editor dialog.

Source: [src/BigCommerce/Container/Editor.php](BigCommerce/Container/Editor.php), [line 137](BigCommerce/Container/Editor.php#L137-L150)

### `bigcommerce/gutenberg/js_config`

Filters the JavaScript configuration for the BigCommerce Gutenberg blocks.

This filter modifies the JavaScript configuration to include the necessary settings
for all registered Gutenberg blocks in the BigCommerce system, based on the available
block types.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | The current JavaScript configuration for Gutenberg blocks.

Source: [src/BigCommerce/Container/Editor.php](BigCommerce/Container/Editor.php), [line 200](BigCommerce/Container/Editor.php#L200-L223)

### `replace_editor`

Checks if the Gutenberg editor should be used for the current post.

This filter determines whether the Gutenberg editor or classic editor should be
used, based on the provided post and the state of the Gutenberg migration process.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`passthrough` | `bool` | Whether to pass through the original value.
`post` | `\BigCommerce\Container\WP_Post` | The current post object.

Source: [src/BigCommerce/Container/Editor.php](BigCommerce/Container/Editor.php), [line 246](BigCommerce/Container/Editor.php#L246-L259)

### `replace_editor`

Checks if the classic editor should be used for the current post.

This filter determines whether the classic editor should be used, based on the
provided post and the state of the Gutenberg migration process.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`passthrough` | `bool` | Whether to pass through the original value.
`post` | `\BigCommerce\Container\WP_Post` | The current post object.

Source: [src/BigCommerce/Container/Editor.php](BigCommerce/Container/Editor.php), [line 261](BigCommerce/Container/Editor.php#L261-L274)

### `bigcommerce/js_config`

Filters JavaScript configuration data to include banners settings.

Modifies the existing JavaScript configuration array to include
any settings or data required by the banners manager.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`config` | `array` | The existing JavaScript configuration.

Source: [src/BigCommerce/Container/Banners.php](BigCommerce/Container/Banners.php), [line 35](BigCommerce/Container/Banners.php#L35-L46)

### `bigcommerce/messages/success/arguments`

Adds tracking attributes to success message arguments after adding a product to the cart.

These attributes are used for tracking events in analytics platforms.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`args` | `array` | Arguments for the success message.
`data` | `array` | Additional data related to the cart event.

Source: [src/BigCommerce/Container/Analytics.php](BigCommerce/Container/Analytics.php), [line 118](BigCommerce/Container/Analytics.php#L118-L130)

### `bigcommerce/button/purchase/attributes`

Adds tracking attributes to the purchase button.

These attributes allow tracking user interactions with the purchase button.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`attributes` | `array` | HTML attributes for the purchase button.
`product` | `object` | The product associated with the button.

Source: [src/BigCommerce/Container/Analytics.php](BigCommerce/Container/Analytics.php), [line 132](BigCommerce/Container/Analytics.php#L132-L144)

### `bigcommerce/template=components/products/view-product-button.php/options`

Adds tracking attributes to the "View Product" button.

These attributes are used to track interactions with product detail links.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`options` | `array` | Options for the view product button.
`template` | `string` | The template path for the button.

Source: [src/BigCommerce/Container/Analytics.php](BigCommerce/Container/Analytics.php), [line 150](BigCommerce/Container/Analytics.php#L150-L162)

### `bigcommerce/template=components/products/product-card.php/options`

Adds tracking attributes to product quick-view buttons on product cards.

Tracks user interactions with quick-view functionality for products.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`options` | `array` | Options for the quick-view button.
`template` | `string` | The template path for the product card.

Source: [src/BigCommerce/Container/Analytics.php](BigCommerce/Container/Analytics.php), [line 164](BigCommerce/Container/Analytics.php#L164-L176)

### `bigcommerce/template=components/products/product-title.php/options`

Adds tracking attributes to product titles.

Tracks user interactions with product title links.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`options` | `array` | Options for the product title link.
`template` | `string` | The template path for the title.

Source: [src/BigCommerce/Container/Analytics.php](BigCommerce/Container/Analytics.php), [line 178](BigCommerce/Container/Analytics.php#L178-L190)

### `BigCommerce\Settings\Sections\Analytics::TRACK_BY_HOOK`

Modifies the tracking data options for analytics.

This allows for customization of analytics tracking behavior.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`track_data` | `array` | Tracking data options.

Source: [src/BigCommerce/Container/Analytics.php](BigCommerce/Container/Analytics.php), [line 192](BigCommerce/Container/Analytics.php#L192-L203)

### `cron_schedules`

Adds a custom cron schedule to the cron schedules.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`schedules` | `array` | The array of existing cron schedules.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 281](BigCommerce/Container/Import.php#L281-L289)

### `bigcommerce_modified_product_ids`

Filter the list of modified product IDs during the BigCommerce import.

This filter allows modification of the product IDs returned for products that have been modified.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`modified_product_ids` | `array` | The list of modified product IDs.
`modified_product_ids` | `array` | The modified product IDs list after applying the filter.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 669](BigCommerce/Container/Import.php#L669-L679)

### `bigcommerce/import/task_list`

Filter the import task list.

This filter modifies the list of tasks to be executed during the import process.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`task_list` | `array` | The list of tasks in the import queue.
`task_list` | `array` | The filtered list of tasks after applying the filter.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 681](BigCommerce/Container/Import.php#L681-L691)

### `bigcommerce/import/term/data`

Filter category data before importing.

This filter modifies the category data based on the BigCommerce category ID.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | The original category data.
`bc_category_id` | `int` | The BigCommerce category ID.
`data` | `array` | The filtered category data after applying the filter.

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 693](BigCommerce/Container/Import.php#L693-L705)

### `bigcommerce/import/product/import_images`

Checks if image import is allowed.

This callback function is hooked into the `bigcommerce/import/product/import_images` filter
to determine whether image import is permitted.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Image.php](BigCommerce/Container/Image.php), [line 28](BigCommerce/Container/Image.php#L28-L38)

### `wp_get_attachment_image`

Modifies the image HTML to load images from CDN if applicable.

This callback function is hooked into the `wp_get_attachment_image` filter to check
if the image should be loaded from a CDN. If a valid BigCommerce ID and CDN URL are found,
the image source is replaced with the CDN URL.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`html` | `string` | The HTML of the image tag.
`thumb_id` | `int` | The attachment ID of the image.

Source: [src/BigCommerce/Container/Image.php](BigCommerce/Container/Image.php), [line 40](BigCommerce/Container/Image.php#L40-L73)

### `bigcommerce/template/directory/plugin`

Look for plugin templates in [plugin]/templates/public.

This filter hooks into the `bigcommerce/template/directory/plugin` event and sets the
plugin template directory to `[plugin]/templates/public` if no directory is provided.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`directory` | `string` | The current plugin template directory.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 53](BigCommerce/Container/Templates.php#L53-L65)

### `bigcommerce/template/directory/theme`

Look for template overrides in [theme]/bigcommerce.

This filter hooks into the `bigcommerce/template/directory/theme` event and sets the
theme template directory to `bigcommerce` if no directory is provided.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`directory` | `string` | The current theme template directory.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 67](BigCommerce/Container/Templates.php#L67-L79)

### `bigcommerce/template/product/single`

Render the product single page template.

This filter hooks into the `bigcommerce/template/product/single` event and checks if a
custom product single template is available. If not, it renders the template using
the `render_product_single` method of the `Template_Override` class.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`output` | `string` | The current output of the product single template.
`post_id` | `int` | The ID of the current product post.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 81](BigCommerce/Container/Templates.php#L81-L99)

### `bigcommerce/template/product/archive`

Render the product archive page template.

This filter hooks into the `bigcommerce/template/product/archive` event and checks if a
custom product archive template is available. If not, it renders the template using
the `render_product_archive` method of the `Template_Override` class.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`output` | `string` | The current output of the product archive template.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 101](BigCommerce/Container/Templates.php#L101-L118)

### `single_template_hierarchy`

Set the product single template path in the template hierarchy.

This filter hooks into the `single_template_hierarchy` event and modifies the template
hierarchy for single product pages by calling the `set_product_single_template_path`
method of the `Template_Override` class.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`templates` | `array` | An array of available templates in the hierarchy.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 124](BigCommerce/Container/Templates.php#L124-L135)

### `singular_template_hierarchy`

Set the singular template path in the template hierarchy.

This filter hooks into the `singular_template_hierarchy` event and modifies the template
hierarchy for singular pages (e.g., single posts or pages) by calling the `set_product_single_template_path`
method of the `Template_Override` class.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`templates` | `array` | An array of available templates in the hierarchy.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 137](BigCommerce/Container/Templates.php#L137-L148)

### `index_template_hierarchy`

Set the index template path in the template hierarchy.

This filter hooks into the `index_template_hierarchy` event and modifies the template
hierarchy for the index page (homepage) by calling the `set_product_single_template_path`
method of the `Template_Override` class.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`templates` | `array` | An array of available templates in the hierarchy.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 150](BigCommerce/Container/Templates.php#L150-L161)

### `archive_template_hierarchy`

Set the product archive template path in the template hierarchy.

This filter hooks into the `archive_template_hierarchy` event and modifies the template
hierarchy for product archive pages by calling the `set_product_archive_template_path`
method of the `Template_Override` class.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`templates` | `array` | An array of available templates in the hierarchy.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 167](BigCommerce/Container/Templates.php#L167-L178)

### `index_template_hierarchy`

Register the template-related services and filters.

This method registers all the necessary services and filters related to templates, including
template overrides, body classes, and template hierarchy modifications. It is called when the
container is initialized and hooks into various WordPress actions and filters for template management.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The container instance used to register services.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 35](BigCommerce/Container/Templates.php#L35-L179)

### `taxonomy_template_hierarchy`

Set the taxonomy archive template path in the template hierarchy.

This filter hooks into the `taxonomy_template_hierarchy` event and modifies the template
hierarchy for taxonomy archive pages by calling the `set_taxonomy_archive_template_path`
method of the `Template_Override` class.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`templates` | `array` | An array of available templates in the hierarchy.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 185](BigCommerce/Container/Templates.php#L185-L196)

### `archive_template_hierarchy`

Set the product archive template path in the template hierarchy.

This filter hooks into the `archive_template_hierarchy` event and modifies the template
hierarchy for product archive pages by calling the `set_product_archive_template_path`
method of the `Template_Override` class.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`templates` | `array` | An array of available templates in the hierarchy.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 198](BigCommerce/Container/Templates.php#L198-L209)

### `index_template_hierarchy`

Register the template-related services and filters.

This method registers all the necessary services and filters related to templates, including
template overrides, body classes, and template hierarchy modifications. It is called when the
container is initialized and hooks into various WordPress actions and filters for template management.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The container instance used to register services.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 35](BigCommerce/Container/Templates.php#L35-L210)

### `search_template_hierarchy`

Set the search template path in the template hierarchy.

This filter hooks into the `search_template_hierarchy` event and modifies the template
hierarchy for search results pages by calling the `set_search_template_path`
method of the `Template_Override` class.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`templates` | `array` | An array of available templates in the hierarchy.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 216](BigCommerce/Container/Templates.php#L216-L227)

### `index_template_hierarchy`

Register the template-related services and filters.

This method registers all the necessary services and filters related to templates, including
template overrides, body classes, and template hierarchy modifications. It is called when the
container is initialized and hooks into various WordPress actions and filters for template management.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `\Pimple\Container` | The container instance used to register services.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 35](BigCommerce/Container/Templates.php#L35-L228)

### `template_include`

Includes the product template if it matches the path.

This filter hooks into the `template_include` event and checks if a custom product template
is available. If so, it includes the template using the `include_product_template`
method of the `Template_Override` class.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`path` | `string` | The current template path.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 230](BigCommerce/Container/Templates.php#L230-L243)

### `body_class`

Add custom body classes.

This filter hooks into the `body_class` event and allows the modification of the body
classes by calling the `set_body_classes` method of the `Body_Classes` class.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`classes` | `array` | An array of the current body classes.

Source: [src/BigCommerce/Container/Templates.php](BigCommerce/Container/Templates.php), [line 245](BigCommerce/Container/Templates.php#L245-L257)

### `get_terms_args`

Exclude product categories by group during term fetching.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`args` | `array` | The arguments for get_terms.
`taxonomies` | `array` | The taxonomies being queried.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 215](BigCommerce/Container/Taxonomies.php#L215-L227)

### `sanitize_option_Channel_Select::CHANNEL_TERM`

Filters the channel selection value when sanitizing options.

This filter modifies the channel selection value before it is saved.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`value` | `mixed` | The channel term value to be sanitized.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 363](BigCommerce/Container/Taxonomies.php#L363-L371)

### `sanitize_option_Channel_Settings::NEW_NAME`

Filters the new channel name when sanitizing options.

This filter modifies the new channel name value before it is saved.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`value` | `mixed` | The new channel name value to be sanitized.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 373](BigCommerce/Container/Taxonomies.php#L373-L381)

### `bigcommerce/settings/api/disabled/field=Api_Credentials::OPTION_STORE_URL`

Filters the store URL changes and prevents them if needed.

This filter prevents changes to the store URL if certain conditions are met.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`disabled` | `bool` | Whether the store URL field is disabled.
`container` | `\Pimple\Container` | The container object.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 383](BigCommerce/Container/Taxonomies.php#L383-L392)

### `restrict_manage_posts`

Adds a channel selection filter to the posts list table for product management in the admin area.

This filter hooks into the `restrict_manage_posts` action, which is triggered when displaying
the posts list table in the WordPress admin. It adds a dropdown menu for selecting a channel,
allowing users to filter products by channel. The filter is displayed for the relevant post type.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_type` | `string` | The post type currently being displayed in the admin area.
`which` | `string` | The screen on which the filter is being displayed (either 'top' or 'bottom').

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 406](BigCommerce/Container/Taxonomies.php#L406-L420)

### `parse_request`

Filters the product list based on the selected channel in the admin area.

This filter hooks into the `parse_request` action, which is triggered when parsing the request
to filter the products list. It applies the channel filter if multichannel is enabled, ensuring
that only the products relevant to the selected channel are displayed.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`wp` | `\WP` | The current WP instance, passed by reference, which contains the query variables.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 422](BigCommerce/Container/Taxonomies.php#L422-L435)

### `bigcommerce/diagnostics`

Adds route-related diagnostics data to the BigCommerce diagnostics.

Modifies the diagnostic data to include information related to routes, as fetched by the `diagnostic_data` method
of the `Routes` class.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | The existing diagnostics data.

Source: [src/BigCommerce/Container/Taxonomies.php](BigCommerce/Container/Taxonomies.php), [line 718](BigCommerce/Container/Taxonomies.php#L718-L730)

### `bigcommerce/product/reviews/rest_url`

Filters the REST URL for product reviews.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The current reviews REST URL.
`post_id` | `int` | The product post ID.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 386](BigCommerce/Container/Rest.php#L386-L396)

### `bigcommerce/js_config`

Filters the BigCommerce JS configuration for cart settings.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`config` | `array` | The existing JS configuration.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 398](BigCommerce/Container/Rest.php#L398-L407)

### `bigcommerce/js_config`

Filters the BigCommerce JS configuration for pricing settings.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`config` | `array` | The existing JS configuration.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 409](BigCommerce/Container/Rest.php#L409-L418)

### `bigcommerce/js_config`

Filters the BigCommerce JS configuration for product settings.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`config` | `array` | The existing JS configuration.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 420](BigCommerce/Container/Rest.php#L420-L429)

### `bigcommerce/js_config`

Filters the BigCommerce JS configuration for shipping settings.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`config` | `array` | The existing JS configuration.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 431](BigCommerce/Container/Rest.php#L431-L440)

### `bigcommerce/js_config`

Filters the BigCommerce JS configuration for coupon code settings.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`config` | `array` | The existing JS configuration.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 442](BigCommerce/Container/Rest.php#L442-L453)

### `bigcommerce/template/path`

Filters the template path for rendering BigCommerce templates.

This allows AMP-specific overrides to adjust the template path dynamically.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`path` | `string` | The original template path.
`relative_path` | `string` | The relative path to the requested template.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 228](BigCommerce/Container/Amp.php#L228-L238)

### `bigcommerce/template/controller_factory`

Filters the controller factory used to load BigCommerce templates.

This allows AMP to replace the default controller factory with an AMP-specific implementation.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`factory` | `object` | The current controller factory.
`classname` | `string` | The class name for the requested controller.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 240](BigCommerce/Container/Amp.php#L240-L249)

### `bigcommerce/template/data`

Filters the template data used for rendering BigCommerce templates.

This adds AMP-specific adjustments, such as ensuring valid AMP-compatible `<img>` elements.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | The data array for the template.
`template` | `string` | The template being rendered.
`options` | `array` | Additional options for the template.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 251](BigCommerce/Container/Amp.php#L251-L262)

### `bigcommerce/button/purchase`

Filters the purchase button markup.

This allows AMP to modify the purchase button for AMP-specific functionality.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`button` | `string` | The original purchase button markup.
`post_id` | `int` | The ID of the product post.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 264](BigCommerce/Container/Amp.php#L264-L274)

### `bigcommerce/template/wrapper/attributes`

Filters the attributes of the template wrapper element.

This removes AMP-incompatible attributes to ensure validation.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`attributes` | `array` | The attributes for the wrapper element.
`template_name` | `string` | The name of the template being rendered.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 276](BigCommerce/Container/Amp.php#L276-L286)

### `bigcommerce/template/image/fallback`

Filters the fallback image used in BigCommerce templates.

This allows AMP to provide a specific fallback image for AMP templates.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 288](BigCommerce/Container/Amp.php#L288-L297)

### `wp_kses_allowed_html`

Filters the allowed HTML tags and attributes for the current context.

This enables AMP to add or remove specific tags and attributes for validation.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`allowed_tags` | `array` | The currently allowed tags and attributes.
`context` | `string` | The context for which tags are allowed.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 299](BigCommerce/Container/Amp.php#L299-L309)

### `amp_post_template_file`

Filters the AMP template file for rendering a post.

This allows overriding the default AMP template file with a classic template.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`file` | `string` | The path to the current template file.
`type` | `string` | The type of template being loaded (e.g., `single`, `archive`).
`post_type` | `string` | The post type being rendered.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 325](BigCommerce/Container/Amp.php#L325-L336)

### `amp_post_template_file`

Filters the AMP template file for rendering the header.

This allows overriding the default header template with a custom AMP-specific version.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`file` | `string` | The path to the current header template file.
`type` | `string` | The type of template being loaded (e.g., `header`).

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 338](BigCommerce/Container/Amp.php#L338-L348)

### `amp_post_template_data`

Filters the data used by AMP post templates.

This enables customization of the rendered data, such as modifying the menu structure for AMP.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | The data array passed to the AMP template.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 350](BigCommerce/Container/Amp.php#L350-L359)

### `bigcommerce/assets/stylesheet`

Filters the stylesheet URL for BigCommerce assets.

This allows modifying or replacing the default stylesheet used by BigCommerce, such as providing AMP-compatible styles.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`stylesheet` | `string` | The URL of the BigCommerce stylesheet.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 362](BigCommerce/Container/Amp.php#L362-L371)

### `wp_setup_nav_menu_item`

Filters a single nav menu item during setup.

This adds custom classes to the nav menu item if it corresponds to the cart page, using data from the BigCommerce container.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`menu_item` | `\BigCommerce\Container\WP_Post` | The menu item being processed.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 374](BigCommerce/Container/Amp.php#L374-L385)

### `amp_post_template_data`

Filters the data passed to AMP post templates.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | The data passed to the post template.

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 404](BigCommerce/Container/Amp.php#L404-L416)

### `page_template`

Filters the page template for custom page types.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`template` | `string` | The current template being used.
`type` | `string` | The type of page (e.g., 'page', 'single', etc.).
`templates` | `array` | Array of available templates.

Source: [src/BigCommerce/Container/Compatibility.php](BigCommerce/Container/Compatibility.php), [line 93](BigCommerce/Container/Compatibility.php#L93-L104)

### `bigcommerce/js_config`

Filters the JS configuration for Matomo tracking.

This filter checks if Matomo is enabled and modifies the JS configuration accordingly.
If tracking is enabled, the Matomo integration adds its own JS configuration.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`config` | `array` | The current JS configuration.

Source: [src/BigCommerce/Container/Compatibility.php](BigCommerce/Container/Compatibility.php), [line 209](BigCommerce/Container/Compatibility.php#L209-L225)

### `bigcommerce/currency/format`

Filters the currency formatting for a given value.

This filter allows modification of how a currency value is formatted. It utilizes
the formatter to convert the value into the correct format based on the active currency.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`formatted` | `string` | The formatted currency value.
`value` | `float` | The raw currency value to be formatted.

Source: [src/BigCommerce/Container/Currency.php](BigCommerce/Container/Currency.php), [line 72](BigCommerce/Container/Currency.php#L72-L85)

### `bigcommerce/currency/code`

Filters the currency code.

This filter allows modification of the currency code being used. It returns
the current currency code based on the configured currency.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Currency.php](BigCommerce/Container/Currency.php), [line 87](BigCommerce/Container/Currency.php#L87-L97)

### `bigcommerce/currency/enabled`

Filters the list of enabled currencies for the current channel.

This filter returns a list of currencies that are enabled for the current channel,
allowing for dynamic adjustment based on context.

**Arguments**

No arguments.

Source: [src/BigCommerce/Container/Currency.php](BigCommerce/Container/Currency.php), [line 99](BigCommerce/Container/Currency.php#L99-L109)

### `pre_option_BigCommerce\Settings\Sections\Cart::OPTION_EMBEDDED_CHECKOUT`

Filters the value of the "Embedded Checkout" option based on setup requirements.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`value` | `mixed` | The current option value.

Source: [src/BigCommerce/Container/Checkout.php](BigCommerce/Container/Checkout.php), [line 69](BigCommerce/Container/Checkout.php#L69-L77)

### `bigcommerce/checkout/can_embed`

Determines whether the embedded checkout can be enabled based on current requirements.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`supported` | `bool` | Indicates if embedded checkout is currently supported.

Source: [src/BigCommerce/Container/Checkout.php](BigCommerce/Container/Checkout.php), [line 79](BigCommerce/Container/Checkout.php#L79-L87)

### `bigcommerce/checkout/url`

Modifies the checkout URL by adding a login token for customer authentication.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The original checkout URL.

Source: [src/BigCommerce/Container/Checkout.php](BigCommerce/Container/Checkout.php), [line 95](BigCommerce/Container/Checkout.php#L95-L103)

### `wp_setup_nav_menu_item`

Filters the setup of a navigation menu item.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`item` | `mixed` | The menu item being set up.

Source: [src/BigCommerce/Container/Nav_Menu.php](BigCommerce/Container/Nav_Menu.php), [line 59](BigCommerce/Container/Nav_Menu.php#L59-L67)

### `wp_get_nav_menu_items`

Filters the list of navigation menu items to include dynamic items.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`items` | `array` | The existing menu items.
`menu` | `object` | The current menu object.
`args` | `array` | The menu arguments.

Source: [src/BigCommerce/Container/Nav_Menu.php](BigCommerce/Container/Nav_Menu.php), [line 69](BigCommerce/Container/Nav_Menu.php#L69-L79)

### `customize_nav_menu_available_item_types`

Filters the available item types in the customizer.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`types` | `array` | The existing item types.

Source: [src/BigCommerce/Container/Nav_Menu.php](BigCommerce/Container/Nav_Menu.php), [line 123](BigCommerce/Container/Nav_Menu.php#L123-L131)

### `customize_nav_menu_available_items`

Filters the available menu items in the customizer.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`items` | `array` | The existing menu items.
`type` | `string` | The item type.
`object` | `object` | The current object.
`page` | `int` | The page number.

Source: [src/BigCommerce/Container/Nav_Menu.php](BigCommerce/Container/Nav_Menu.php), [line 133](BigCommerce/Container/Nav_Menu.php#L133-L144)

### `pre_option_Currency::CURRENCY_CODE`

Temporarily filters the currency code to match the order's currency.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`currency` | `string` | The original currency code.

Source: [src/BigCommerce/Shortcodes/Order_History.php](BigCommerce/Shortcodes/Order_History.php), [line 110](BigCommerce/Shortcodes/Order_History.php#L110-L117)

### `pre_option_Currency::CURRENCY_CODE`

Temporarily filters the currency code to match the order's currency.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`currency` | `string` | The original currency code.

Source: [src/BigCommerce/Shortcodes/Order_History.php](BigCommerce/Shortcodes/Order_History.php), [line 140](BigCommerce/Shortcodes/Order_History.php#L140-L147)


<p align="center"><a href="https://github.com/pronamic/wp-documentor"><img src="https://cdn.jsdelivr.net/gh/pronamic/wp-documentor@main/logos/pronamic-wp-documentor.svgo-min.svg" alt="Pronamic WordPress Documentor" width="32" height="32"></a><br><em>Generated by <a href="https://github.com/pronamic/wp-documentor">Pronamic WordPress Documentor</a> <code>1.2.0</code></em><p>

