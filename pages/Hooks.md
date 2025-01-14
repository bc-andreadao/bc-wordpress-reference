# Hooks

- [Actions](#actions)
- [Filters](#filters)

## Actions

### bigcommerce/proxy/cache_set


Fires when a result has been cached.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`result` | `array\|\WP_Error` | Result from API call.
`request` | `\WP_REST_Request` | API request.

Source: [src/BigCommerce/Proxy/Proxy_Cache.php](BigCommerce/Proxy/Proxy_Cache.php), [line 165](BigCommerce/Proxy/Proxy_Cache.php#L165-L171)

### bigcommerce/proxy/cache_get


Result retrieved from cache.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`result` | `array` | Result returned from cache.
`request` | `\WP_REST_Request` | API request.

Source: [src/BigCommerce/Proxy/Proxy_Cache.php](BigCommerce/Proxy/Proxy_Cache.php), [line 220](BigCommerce/Proxy/Proxy_Cache.php#L220-L226)

### bigcommerce/proxy/request_received


Fires before a proxy REST request is run.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`request` | `\WP_REST_Request` | API request.

Source: [src/BigCommerce/Proxy/Proxy_Controller.php](BigCommerce/Proxy/Proxy_Controller.php), [line 331](BigCommerce/Proxy/Proxy_Controller.php#L331-L336)

### bigcommerce/proxy/raw_response_received


Raw API response received.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`response` | `object\|array` | Response from BigCommerce API.
`route` | `string` | Route requested.
`request` | `\WP_REST_Request` | API request.

Source: [src/BigCommerce/Proxy/Proxy_Controller.php](BigCommerce/Proxy/Proxy_Controller.php), [line 363](BigCommerce/Proxy/Proxy_Controller.php#L363-L370)

### bigcommerce/proxy/response_received


Do something with the response before it is returned. E.g. Import the product(s) and/or cache it.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`result` | `array\|\WP_Error` | Result from API call.
`request` | `\WP_REST_Request` | API request.

Source: [src/BigCommerce/Proxy/Proxy_Controller.php](BigCommerce/Proxy/Proxy_Controller.php), [line 379](BigCommerce/Proxy/Proxy_Controller.php#L379-L385)

### bigcommerce/form/error


Fires when there is an error processing the add to cart form.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`error` | `\WP_Error` | The error object
`submission` | `array` | The submitted form data
`redirect` | `string` | The URL to redirect to after handling submission
`data` | `array` | Additional data about the submission

Source: [src/BigCommerce/Cart/Add_To_Cart.php](BigCommerce/Cart/Add_To_Cart.php), [line 28](BigCommerce/Cart/Add_To_Cart.php#L28-L36)

Source: [src/BigCommerce/Cart/Add_To_Cart.php](BigCommerce/Cart/Add_To_Cart.php), [line 156](BigCommerce/Cart/Add_To_Cart.php#L156-L164)

Source: [src/BigCommerce/Cart/Buy_Now.php](BigCommerce/Cart/Buy_Now.php), [line 69](BigCommerce/Cart/Buy_Now.php#L69-L80)

Source: [src/BigCommerce/Cart/Cart_Recovery.php](BigCommerce/Cart/Cart_Recovery.php), [line 86](BigCommerce/Cart/Cart_Recovery.php#L86-L93)

Source: [src/BigCommerce/Cart/Checkout.php](BigCommerce/Cart/Checkout.php), [line 55](BigCommerce/Cart/Checkout.php#L55-L62)

Source: [src/BigCommerce/Cart/Checkout.php](BigCommerce/Cart/Checkout.php), [line 88](BigCommerce/Cart/Checkout.php#L88-L95)

Source: [src/BigCommerce/Forms/Update_Address_Handler.php](BigCommerce/Forms/Update_Address_Handler.php), [line 43](BigCommerce/Forms/Update_Address_Handler.php#L43-L43)

Source: [src/BigCommerce/Forms/Update_Address_Handler.php](BigCommerce/Forms/Update_Address_Handler.php), [line 60](BigCommerce/Forms/Update_Address_Handler.php#L60-L60)

Source: [src/BigCommerce/Forms/Delete_Address_Handler.php](BigCommerce/Forms/Delete_Address_Handler.php), [line 33](BigCommerce/Forms/Delete_Address_Handler.php#L33-L40)

Source: [src/BigCommerce/Forms/Registration_Handler.php](BigCommerce/Forms/Registration_Handler.php), [line 76](BigCommerce/Forms/Registration_Handler.php#L76-L82)

Source: [src/BigCommerce/Forms/Registration_Handler.php](BigCommerce/Forms/Registration_Handler.php), [line 112](BigCommerce/Forms/Registration_Handler.php#L112-L112)

Source: [src/BigCommerce/Forms/Switch_Currency_Handler.php](BigCommerce/Forms/Switch_Currency_Handler.php), [line 75](BigCommerce/Forms/Switch_Currency_Handler.php#L75-L75)

Source: [src/BigCommerce/Forms/Product_Review_Handler.php](BigCommerce/Forms/Product_Review_Handler.php), [line 52](BigCommerce/Forms/Product_Review_Handler.php#L52-L58)

Source: [src/BigCommerce/Forms/Product_Review_Handler.php](BigCommerce/Forms/Product_Review_Handler.php), [line 85](BigCommerce/Forms/Product_Review_Handler.php#L85-L91)

Source: [src/BigCommerce/Forms/Update_Profile_Handler.php](BigCommerce/Forms/Update_Profile_Handler.php), [line 43](BigCommerce/Forms/Update_Profile_Handler.php#L43-L43)

Source: [src/BigCommerce/Forms/Update_Profile_Handler.php](BigCommerce/Forms/Update_Profile_Handler.php), [line 79](BigCommerce/Forms/Update_Profile_Handler.php#L79-L79)

Source: [src/BigCommerce/Forms/Update_Profile_Handler.php](BigCommerce/Forms/Update_Profile_Handler.php), [line 88](BigCommerce/Forms/Update_Profile_Handler.php#L88-L88)

Source: [src/BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php), [line 72](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php#L72-L78)

Source: [src/BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php), [line 105](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php#L105-L105)

Source: [src/BigCommerce/Accounts/Wishlists/Actions/Edit_Wishlist.php](BigCommerce/Accounts/Wishlists/Actions/Edit_Wishlist.php), [line 64](BigCommerce/Accounts/Wishlists/Actions/Edit_Wishlist.php#L64-L72)

Source: [src/BigCommerce/Accounts/Wishlists/Actions/Add_Item.php](BigCommerce/Accounts/Wishlists/Actions/Add_Item.php), [line 78](BigCommerce/Accounts/Wishlists/Actions/Add_Item.php#L78-L86)

Source: [src/BigCommerce/Accounts/Wishlists/Actions/Create_Wishlist.php](BigCommerce/Accounts/Wishlists/Actions/Create_Wishlist.php), [line 67](BigCommerce/Accounts/Wishlists/Actions/Create_Wishlist.php#L67-L75)

Source: [src/BigCommerce/Accounts/Wishlists/Actions/Delete_Wishlist.php](BigCommerce/Accounts/Wishlists/Actions/Delete_Wishlist.php), [line 55](BigCommerce/Accounts/Wishlists/Actions/Delete_Wishlist.php#L55-L63)

Source: [src/BigCommerce/Accounts/Wishlists/Actions/Remove_Item.php](BigCommerce/Accounts/Wishlists/Actions/Remove_Item.php), [line 81](BigCommerce/Accounts/Wishlists/Actions/Remove_Item.php#L81-L89)

### bigcommerce/form/success


Triggered when a form is successfully processed.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`message` | `string` | The message that will display to the user.
`submission` | `array` | The data submitted to the form.
`url` | `string` | The URL to redirect the user to.
`data` | `array` | Additional data to store with the message.

Source: [src/BigCommerce/Cart/Add_To_Cart.php](BigCommerce/Cart/Add_To_Cart.php), [line 109](BigCommerce/Cart/Add_To_Cart.php#L109-L123)

Source: [src/BigCommerce/Forms/Update_Address_Handler.php](BigCommerce/Forms/Update_Address_Handler.php), [line 72](BigCommerce/Forms/Update_Address_Handler.php#L72-L72)

Source: [src/BigCommerce/Forms/Update_Address_Handler.php](BigCommerce/Forms/Update_Address_Handler.php), [line 80](BigCommerce/Forms/Update_Address_Handler.php#L80-L80)

Source: [src/BigCommerce/Forms/Delete_Address_Handler.php](BigCommerce/Forms/Delete_Address_Handler.php), [line 49](BigCommerce/Forms/Delete_Address_Handler.php#L49-L59)

Source: [src/BigCommerce/Forms/Registration_Handler.php](BigCommerce/Forms/Registration_Handler.php), [line 177](BigCommerce/Forms/Registration_Handler.php#L177-L185)

Source: [src/BigCommerce/Forms/Switch_Currency_Handler.php](BigCommerce/Forms/Switch_Currency_Handler.php), [line 104](BigCommerce/Forms/Switch_Currency_Handler.php#L104-L112)

Source: [src/BigCommerce/Forms/Product_Review_Handler.php](BigCommerce/Forms/Product_Review_Handler.php), [line 102](BigCommerce/Forms/Product_Review_Handler.php#L102-L109)

Source: [src/BigCommerce/Forms/Update_Profile_Handler.php](BigCommerce/Forms/Update_Profile_Handler.php), [line 99](BigCommerce/Forms/Update_Profile_Handler.php#L99-L99)

Source: [src/BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php), [line 126](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php#L126-L133)

Source: [src/BigCommerce/Accounts/Wishlists/Actions/Edit_Wishlist.php](BigCommerce/Accounts/Wishlists/Actions/Edit_Wishlist.php), [line 54](BigCommerce/Accounts/Wishlists/Actions/Edit_Wishlist.php#L54-L62)

Source: [src/BigCommerce/Accounts/Wishlists/Actions/Add_Item.php](BigCommerce/Accounts/Wishlists/Actions/Add_Item.php), [line 68](BigCommerce/Accounts/Wishlists/Actions/Add_Item.php#L68-L76)

Source: [src/BigCommerce/Accounts/Wishlists/Actions/Create_Wishlist.php](BigCommerce/Accounts/Wishlists/Actions/Create_Wishlist.php), [line 57](BigCommerce/Accounts/Wishlists/Actions/Create_Wishlist.php#L57-L65)

Source: [src/BigCommerce/Accounts/Wishlists/Actions/Delete_Wishlist.php](BigCommerce/Accounts/Wishlists/Actions/Delete_Wishlist.php), [line 45](BigCommerce/Accounts/Wishlists/Actions/Delete_Wishlist.php#L45-L53)

Source: [src/BigCommerce/Accounts/Wishlists/Actions/Remove_Item.php](BigCommerce/Accounts/Wishlists/Actions/Remove_Item.php), [line 71](BigCommerce/Accounts/Wishlists/Actions/Remove_Item.php#L71-L79)

### bigcommerce/do_not_cache


Fires when a BigCommerce shortcode is detected in the post content.

This action triggers cache prevention mechanisms to ensure dynamic cart content is always fresh.

**Arguments**

No arguments.

Source: [src/BigCommerce/Cart/Cache_Control.php](BigCommerce/Cart/Cache_Control.php), [line 30](BigCommerce/Cart/Cache_Control.php#L30-L34)

### bigcommerce/form/before_redirect


Fires immediately before redirecting the user after a form submission.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The destination URL of the redirect.

Source: [src/BigCommerce/Forms/Form_Redirect.php](BigCommerce/Forms/Form_Redirect.php), [line 34](BigCommerce/Forms/Form_Redirect.php#L34-L39)

### bigcommerce/form/redirect


Fires when a form is about to redirect due to an error.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The URL to redirect to, with error parameters added.

Source: [src/BigCommerce/Forms/Error_Handler.php](BigCommerce/Forms/Error_Handler.php), [line 43](BigCommerce/Forms/Error_Handler.php#L43-L48)

Source: [src/BigCommerce/Forms/Success_Handler.php](BigCommerce/Forms/Success_Handler.php), [line 54](BigCommerce/Forms/Success_Handler.php#L54-L59)

### bigcommerce/log


Action to log messages during the BigCommerce logging process.

This action is triggered when a log entry needs to be created. It logs the message, context, level, and path to the log file.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`level` | `string` | The log level (e.g., INFO, ERROR).
`message` | `string` | The log message to be recorded.
`context` | `array` | Additional context for the log entry.
`path` | `string` | The path where the log is being written.

Source: [src/BigCommerce/GraphQL/BaseGQL.php](BigCommerce/GraphQL/BaseGQL.php), [line 151](BigCommerce/GraphQL/BaseGQL.php#L151-L164)

Source: [src/BigCommerce/GraphQL/BaseGQL.php](BigCommerce/GraphQL/BaseGQL.php), [line 193](BigCommerce/GraphQL/BaseGQL.php#L193-L195)

Source: [src/BigCommerce/Import/Task_Manager.php](BigCommerce/Import/Task_Manager.php), [line 93](BigCommerce/Import/Task_Manager.php#L93-L96)

Source: [src/BigCommerce/Import/Task_Manager.php](BigCommerce/Import/Task_Manager.php), [line 101](BigCommerce/Import/Task_Manager.php#L101-L104)

Source: [src/BigCommerce/Import/Task_Manager.php](BigCommerce/Import/Task_Manager.php), [line 105](BigCommerce/Import/Task_Manager.php#L105-L105)

Source: [src/BigCommerce/Import/Task_Manager.php](BigCommerce/Import/Task_Manager.php), [line 129](BigCommerce/Import/Task_Manager.php#L129-L129)

Source: [src/BigCommerce/Import/Processors/Deleted_Product_Marker.php](BigCommerce/Import/Processors/Deleted_Product_Marker.php), [line 69](BigCommerce/Import/Processors/Deleted_Product_Marker.php#L69-L71)

Source: [src/BigCommerce/Import/Processors/Deleted_Product_Marker.php](BigCommerce/Import/Processors/Deleted_Product_Marker.php), [line 88](BigCommerce/Import/Processors/Deleted_Product_Marker.php#L88-L91)

Source: [src/BigCommerce/Import/Processors/Storefront_Processor.php](BigCommerce/Import/Processors/Storefront_Processor.php), [line 54](BigCommerce/Import/Processors/Storefront_Processor.php#L54-L54)

Source: [src/BigCommerce/Import/Processors/Storefront_Processor.php](BigCommerce/Import/Processors/Storefront_Processor.php), [line 59](BigCommerce/Import/Processors/Storefront_Processor.php#L59-L59)

Source: [src/BigCommerce/Import/Processors/Storefront_Processor.php](BigCommerce/Import/Processors/Storefront_Processor.php), [line 84](BigCommerce/Import/Processors/Storefront_Processor.php#L84-L84)

Source: [src/BigCommerce/Import/Processors/Storefront_Processor.php](BigCommerce/Import/Processors/Storefront_Processor.php), [line 89](BigCommerce/Import/Processors/Storefront_Processor.php#L89-L91)

Source: [src/BigCommerce/Import/Processors/Storefront_Processor.php](BigCommerce/Import/Processors/Storefront_Processor.php), [line 110](BigCommerce/Import/Processors/Storefront_Processor.php#L110-L114)

Source: [src/BigCommerce/Import/Processors/Storefront_Processor.php](BigCommerce/Import/Processors/Storefront_Processor.php), [line 118](BigCommerce/Import/Processors/Storefront_Processor.php#L118-L120)

Source: [src/BigCommerce/Import/Processors/Storefront_Processor.php](BigCommerce/Import/Processors/Storefront_Processor.php), [line 139](BigCommerce/Import/Processors/Storefront_Processor.php#L139-L141)

Source: [src/BigCommerce/Import/Processors/Storefront_Processor.php](BigCommerce/Import/Processors/Storefront_Processor.php), [line 146](BigCommerce/Import/Processors/Storefront_Processor.php#L146-L148)

Source: [src/BigCommerce/Import/Processors/Storefront_Processor.php](BigCommerce/Import/Processors/Storefront_Processor.php), [line 157](BigCommerce/Import/Processors/Storefront_Processor.php#L157-L161)

Source: [src/BigCommerce/Import/Processors/Storefront_Processor.php](BigCommerce/Import/Processors/Storefront_Processor.php), [line 165](BigCommerce/Import/Processors/Storefront_Processor.php#L165-L167)

Source: [src/BigCommerce/Import/Processors/Storefront_Processor.php](BigCommerce/Import/Processors/Storefront_Processor.php), [line 185](BigCommerce/Import/Processors/Storefront_Processor.php#L185-L185)

Source: [src/BigCommerce/Import/Processors/Storefront_Processor.php](BigCommerce/Import/Processors/Storefront_Processor.php), [line 190](BigCommerce/Import/Processors/Storefront_Processor.php#L190-L192)

Source: [src/BigCommerce/Import/Processors/Storefront_Processor.php](BigCommerce/Import/Processors/Storefront_Processor.php), [line 202](BigCommerce/Import/Processors/Storefront_Processor.php#L202-L206)

Source: [src/BigCommerce/Import/Processors/Storefront_Processor.php](BigCommerce/Import/Processors/Storefront_Processor.php), [line 210](BigCommerce/Import/Processors/Storefront_Processor.php#L210-L212)

Source: [src/BigCommerce/Import/Processors/Term_Purge.php](BigCommerce/Import/Processors/Term_Purge.php), [line 75](BigCommerce/Import/Processors/Term_Purge.php#L75-L79)

Source: [src/BigCommerce/Import/Processors/Term_Purge.php](BigCommerce/Import/Processors/Term_Purge.php), [line 96](BigCommerce/Import/Processors/Term_Purge.php#L96-L96)

Source: [src/BigCommerce/Import/Processors/Term_Purge.php](BigCommerce/Import/Processors/Term_Purge.php), [line 105](BigCommerce/Import/Processors/Term_Purge.php#L105-L107)

Source: [src/BigCommerce/Import/Processors/Term_Purge.php](BigCommerce/Import/Processors/Term_Purge.php), [line 115](BigCommerce/Import/Processors/Term_Purge.php#L115-L118)

Source: [src/BigCommerce/Import/Processors/Headless_Product_Processor.php](BigCommerce/Import/Processors/Headless_Product_Processor.php), [line 74](BigCommerce/Import/Processors/Headless_Product_Processor.php#L74-L74)

Source: [src/BigCommerce/Import/Processors/Headless_Product_Processor.php](BigCommerce/Import/Processors/Headless_Product_Processor.php), [line 91](BigCommerce/Import/Processors/Headless_Product_Processor.php#L91-L91)

Source: [src/BigCommerce/Import/Processors/Headless_Product_Processor.php](BigCommerce/Import/Processors/Headless_Product_Processor.php), [line 136](BigCommerce/Import/Processors/Headless_Product_Processor.php#L136-L136)

Source: [src/BigCommerce/Import/Processors/Headless_Product_Processor.php](BigCommerce/Import/Processors/Headless_Product_Processor.php), [line 158](BigCommerce/Import/Processors/Headless_Product_Processor.php#L158-L161)

Source: [src/BigCommerce/Import/Processors/Headless_Product_Processor.php](BigCommerce/Import/Processors/Headless_Product_Processor.php), [line 166](BigCommerce/Import/Processors/Headless_Product_Processor.php#L166-L168)

Source: [src/BigCommerce/Import/Processors/Headless_Product_Processor.php](BigCommerce/Import/Processors/Headless_Product_Processor.php), [line 177](BigCommerce/Import/Processors/Headless_Product_Processor.php#L177-L179)

Source: [src/BigCommerce/Import/Processors/Default_Customer_Group.php](BigCommerce/Import/Processors/Default_Customer_Group.php), [line 67](BigCommerce/Import/Processors/Default_Customer_Group.php#L67-L69)

Source: [src/BigCommerce/Import/Processors/Default_Customer_Group.php](BigCommerce/Import/Processors/Default_Customer_Group.php), [line 93](BigCommerce/Import/Processors/Default_Customer_Group.php#L93-L96)

Source: [src/BigCommerce/Import/Processors/Default_Customer_Group.php](BigCommerce/Import/Processors/Default_Customer_Group.php), [line 110](BigCommerce/Import/Processors/Default_Customer_Group.php#L110-L110)

Source: [src/BigCommerce/Import/Processors/Store_Settings.php](BigCommerce/Import/Processors/Store_Settings.php), [line 63](BigCommerce/Import/Processors/Store_Settings.php#L63-L63)

Source: [src/BigCommerce/Import/Processors/Store_Settings.php](BigCommerce/Import/Processors/Store_Settings.php), [line 99](BigCommerce/Import/Processors/Store_Settings.php#L99-L101)

Source: [src/BigCommerce/Import/Processors/Store_Settings.php](BigCommerce/Import/Processors/Store_Settings.php), [line 149](BigCommerce/Import/Processors/Store_Settings.php#L149-L152)

Source: [src/BigCommerce/Import/Processors/Store_Settings.php](BigCommerce/Import/Processors/Store_Settings.php), [line 165](BigCommerce/Import/Processors/Store_Settings.php#L165-L165)

Source: [src/BigCommerce/Import/Processors/Store_Settings.php](BigCommerce/Import/Processors/Store_Settings.php), [line 178](BigCommerce/Import/Processors/Store_Settings.php#L178-L178)

Source: [src/BigCommerce/Import/Processors/Brand_Import.php](BigCommerce/Import/Processors/Brand_Import.php), [line 131](BigCommerce/Import/Processors/Brand_Import.php#L131-L134)

Source: [src/BigCommerce/Import/Processors/Brand_Import.php](BigCommerce/Import/Processors/Brand_Import.php), [line 136](BigCommerce/Import/Processors/Brand_Import.php#L136-L136)

Source: [src/BigCommerce/Import/Processors/Product_Data_Fetcher.php](BigCommerce/Import/Processors/Product_Data_Fetcher.php), [line 49](BigCommerce/Import/Processors/Product_Data_Fetcher.php#L49-L52)

Source: [src/BigCommerce/Import/Processors/Product_Data_Fetcher.php](BigCommerce/Import/Processors/Product_Data_Fetcher.php), [line 60](BigCommerce/Import/Processors/Product_Data_Fetcher.php#L60-L60)

Source: [src/BigCommerce/Import/Processors/Product_Data_Fetcher.php](BigCommerce/Import/Processors/Product_Data_Fetcher.php), [line 67](BigCommerce/Import/Processors/Product_Data_Fetcher.php#L67-L70)

Source: [src/BigCommerce/Import/Processors/Product_Data_Fetcher.php](BigCommerce/Import/Processors/Product_Data_Fetcher.php), [line 78](BigCommerce/Import/Processors/Product_Data_Fetcher.php#L78-L83)

Source: [src/BigCommerce/Import/Processors/Product_Data_Fetcher.php](BigCommerce/Import/Processors/Product_Data_Fetcher.php), [line 85](BigCommerce/Import/Processors/Product_Data_Fetcher.php#L85-L85)

Source: [src/BigCommerce/Import/Processors/Product_Data_Fetcher.php](BigCommerce/Import/Processors/Product_Data_Fetcher.php), [line 90](BigCommerce/Import/Processors/Product_Data_Fetcher.php#L90-L90)

Source: [src/BigCommerce/Import/Processors/Product_Data_Fetcher.php](BigCommerce/Import/Processors/Product_Data_Fetcher.php), [line 91](BigCommerce/Import/Processors/Product_Data_Fetcher.php#L91-L94)

Source: [src/BigCommerce/Import/Processors/Product_Data_Fetcher.php](BigCommerce/Import/Processors/Product_Data_Fetcher.php), [line 127](BigCommerce/Import/Processors/Product_Data_Fetcher.php#L127-L129)

Source: [src/BigCommerce/Import/Processors/Product_Data_Fetcher.php](BigCommerce/Import/Processors/Product_Data_Fetcher.php), [line 151](BigCommerce/Import/Processors/Product_Data_Fetcher.php#L151-L154)

Source: [src/BigCommerce/Import/Processors/Product_Data_Fetcher.php](BigCommerce/Import/Processors/Product_Data_Fetcher.php), [line 183](BigCommerce/Import/Processors/Product_Data_Fetcher.php#L183-L185)

Source: [src/BigCommerce/Import/Processors/Currencies.php](BigCommerce/Import/Processors/Currencies.php), [line 68](BigCommerce/Import/Processors/Currencies.php#L68-L68)

Source: [src/BigCommerce/Import/Processors/Currencies.php](BigCommerce/Import/Processors/Currencies.php), [line 105](BigCommerce/Import/Processors/Currencies.php#L105-L105)

Source: [src/BigCommerce/Import/Processors/Currencies.php](BigCommerce/Import/Processors/Currencies.php), [line 108](BigCommerce/Import/Processors/Currencies.php#L108-L110)

Source: [src/BigCommerce/Import/Processors/Currencies.php](BigCommerce/Import/Processors/Currencies.php), [line 114](BigCommerce/Import/Processors/Currencies.php#L114-L118)

Source: [src/BigCommerce/Import/Processors/Currencies.php](BigCommerce/Import/Processors/Currencies.php), [line 122](BigCommerce/Import/Processors/Currencies.php#L122-L126)

Source: [src/BigCommerce/Import/Processors/Queue_Runner.php](BigCommerce/Import/Processors/Queue_Runner.php), [line 69](BigCommerce/Import/Processors/Queue_Runner.php#L69-L71)

Source: [src/BigCommerce/Import/Processors/Queue_Runner.php](BigCommerce/Import/Processors/Queue_Runner.php), [line 86](BigCommerce/Import/Processors/Queue_Runner.php#L86-L89)

Source: [src/BigCommerce/Import/Processors/Queue_Runner.php](BigCommerce/Import/Processors/Queue_Runner.php), [line 90](BigCommerce/Import/Processors/Queue_Runner.php#L90-L90)

Source: [src/BigCommerce/Import/Processors/Queue_Runner.php](BigCommerce/Import/Processors/Queue_Runner.php), [line 100](BigCommerce/Import/Processors/Queue_Runner.php#L100-L103)

Source: [src/BigCommerce/Import/Processors/Queue_Runner.php](BigCommerce/Import/Processors/Queue_Runner.php), [line 120](BigCommerce/Import/Processors/Queue_Runner.php#L120-L123)

Source: [src/BigCommerce/Import/Processors/Queue_Runner.php](BigCommerce/Import/Processors/Queue_Runner.php), [line 128](BigCommerce/Import/Processors/Queue_Runner.php#L128-L133)

Source: [src/BigCommerce/Import/Processors/Queue_Runner.php](BigCommerce/Import/Processors/Queue_Runner.php), [line 150](BigCommerce/Import/Processors/Queue_Runner.php#L150-L152)

Source: [src/BigCommerce/Import/Processors/Queue_Runner.php](BigCommerce/Import/Processors/Queue_Runner.php), [line 171](BigCommerce/Import/Processors/Queue_Runner.php#L171-L174)

Source: [src/BigCommerce/Import/Processors/Queue_Runner.php](BigCommerce/Import/Processors/Queue_Runner.php), [line 185](BigCommerce/Import/Processors/Queue_Runner.php#L185-L188)

Source: [src/BigCommerce/Import/Processors/Queue_Runner.php](BigCommerce/Import/Processors/Queue_Runner.php), [line 195](BigCommerce/Import/Processors/Queue_Runner.php#L195-L199)

Source: [src/BigCommerce/Import/Processors/Queue_Runner.php](BigCommerce/Import/Processors/Queue_Runner.php), [line 210](BigCommerce/Import/Processors/Queue_Runner.php#L210-L213)

Source: [src/BigCommerce/Import/Processors/Queue_Runner.php](BigCommerce/Import/Processors/Queue_Runner.php), [line 224](BigCommerce/Import/Processors/Queue_Runner.php#L224-L226)

Source: [src/BigCommerce/Import/Processors/ProductCleanup.php](BigCommerce/Import/Processors/ProductCleanup.php), [line 72](BigCommerce/Import/Processors/ProductCleanup.php#L72-L74)

Source: [src/BigCommerce/Import/Processors/ProductCleanup.php](BigCommerce/Import/Processors/ProductCleanup.php), [line 79](BigCommerce/Import/Processors/ProductCleanup.php#L79-L79)

Source: [src/BigCommerce/Import/Processors/Category_Import.php](BigCommerce/Import/Processors/Category_Import.php), [line 57](BigCommerce/Import/Processors/Category_Import.php#L57-L57)

Source: [src/BigCommerce/Import/Processors/Category_Import.php](BigCommerce/Import/Processors/Category_Import.php), [line 80](BigCommerce/Import/Processors/Category_Import.php#L80-L80)

Source: [src/BigCommerce/Import/Processors/Category_Import.php](BigCommerce/Import/Processors/Category_Import.php), [line 89](BigCommerce/Import/Processors/Category_Import.php#L89-L89)

Source: [src/BigCommerce/Import/Processors/Category_Import.php](BigCommerce/Import/Processors/Category_Import.php), [line 93](BigCommerce/Import/Processors/Category_Import.php#L93-L93)

Source: [src/BigCommerce/Import/Processors/Category_Import.php](BigCommerce/Import/Processors/Category_Import.php), [line 97](BigCommerce/Import/Processors/Category_Import.php#L97-L97)

Source: [src/BigCommerce/Import/Processors/Category_Import.php](BigCommerce/Import/Processors/Category_Import.php), [line 101](BigCommerce/Import/Processors/Category_Import.php#L101-L101)

Source: [src/BigCommerce/Import/Processors/Category_Import.php](BigCommerce/Import/Processors/Category_Import.php), [line 106](BigCommerce/Import/Processors/Category_Import.php#L106-L106)

Source: [src/BigCommerce/Import/Processors/Category_Import.php](BigCommerce/Import/Processors/Category_Import.php), [line 121](BigCommerce/Import/Processors/Category_Import.php#L121-L121)

Source: [src/BigCommerce/Import/Processors/Start_Import.php](BigCommerce/Import/Processors/Start_Import.php), [line 12](BigCommerce/Import/Processors/Start_Import.php#L12-L12)

Source: [src/BigCommerce/Import/Processors/Channel_Initializer.php](BigCommerce/Import/Processors/Channel_Initializer.php), [line 105](BigCommerce/Import/Processors/Channel_Initializer.php#L105-L108)

Source: [src/BigCommerce/Import/Processors/Channel_Initializer.php](BigCommerce/Import/Processors/Channel_Initializer.php), [line 146](BigCommerce/Import/Processors/Channel_Initializer.php#L146-L146)

Source: [src/BigCommerce/Import/Processors/Channel_Initializer.php](BigCommerce/Import/Processors/Channel_Initializer.php), [line 155](BigCommerce/Import/Processors/Channel_Initializer.php#L155-L155)

Source: [src/BigCommerce/Import/Processors/Channel_Initializer.php](BigCommerce/Import/Processors/Channel_Initializer.php), [line 164](BigCommerce/Import/Processors/Channel_Initializer.php#L164-L167)

Source: [src/BigCommerce/Import/Processors/Channel_Initializer.php](BigCommerce/Import/Processors/Channel_Initializer.php), [line 181](BigCommerce/Import/Processors/Channel_Initializer.php#L181-L181)

Source: [src/BigCommerce/Import/Processors/Channel_Initializer.php](BigCommerce/Import/Processors/Channel_Initializer.php), [line 199](BigCommerce/Import/Processors/Channel_Initializer.php#L199-L202)

Source: [src/BigCommerce/Import/Processors/Channel_Initializer.php](BigCommerce/Import/Processors/Channel_Initializer.php), [line 209](BigCommerce/Import/Processors/Channel_Initializer.php#L209-L212)

Source: [src/BigCommerce/Import/Processors/Channel_Initializer.php](BigCommerce/Import/Processors/Channel_Initializer.php), [line 235](BigCommerce/Import/Processors/Channel_Initializer.php#L235-L237)

Source: [src/BigCommerce/Import/Processors/Channel_Initializer.php](BigCommerce/Import/Processors/Channel_Initializer.php), [line 250](BigCommerce/Import/Processors/Channel_Initializer.php#L250-L250)

Source: [src/BigCommerce/Import/Processors/Channel_Initializer.php](BigCommerce/Import/Processors/Channel_Initializer.php), [line 258](BigCommerce/Import/Processors/Channel_Initializer.php#L258-L260)

Source: [src/BigCommerce/Import/Processors/Image_Resizer.php](BigCommerce/Import/Processors/Image_Resizer.php), [line 40](BigCommerce/Import/Processors/Image_Resizer.php#L40-L40)

Source: [src/BigCommerce/Import/Processors/Image_Resizer.php](BigCommerce/Import/Processors/Image_Resizer.php), [line 42](BigCommerce/Import/Processors/Image_Resizer.php#L42-L45)

Source: [src/BigCommerce/Import/Processors/Image_Resizer.php](BigCommerce/Import/Processors/Image_Resizer.php), [line 63](BigCommerce/Import/Processors/Image_Resizer.php#L63-L66)

Source: [src/BigCommerce/Import/Processors/Image_Resizer.php](BigCommerce/Import/Processors/Image_Resizer.php), [line 74](BigCommerce/Import/Processors/Image_Resizer.php#L74-L77)

Source: [src/BigCommerce/Import/Processors/Image_Resizer.php](BigCommerce/Import/Processors/Image_Resizer.php), [line 83](BigCommerce/Import/Processors/Image_Resizer.php#L83-L85)

Source: [src/BigCommerce/Import/Processors/Term_Import.php](BigCommerce/Import/Processors/Term_Import.php), [line 114](BigCommerce/Import/Processors/Term_Import.php#L114-L117)

Source: [src/BigCommerce/Import/Processors/Term_Import.php](BigCommerce/Import/Processors/Term_Import.php), [line 129](BigCommerce/Import/Processors/Term_Import.php#L129-L132)

Source: [src/BigCommerce/Import/Processors/Term_Import.php](BigCommerce/Import/Processors/Term_Import.php), [line 139](BigCommerce/Import/Processors/Term_Import.php#L139-L139)

Source: [src/BigCommerce/Import/Processors/Cleanup.php](BigCommerce/Import/Processors/Cleanup.php), [line 114](BigCommerce/Import/Processors/Cleanup.php#L114-L114)

Source: [src/BigCommerce/Import/Processors/Cleanup.php](BigCommerce/Import/Processors/Cleanup.php), [line 138](BigCommerce/Import/Processors/Cleanup.php#L138-L138)

Source: [src/BigCommerce/Import/Processors/Cleanup.php](BigCommerce/Import/Processors/Cleanup.php), [line 141](BigCommerce/Import/Processors/Cleanup.php#L141-L143)

Source: [src/BigCommerce/Import/Processors/Listing_Fetcher.php](BigCommerce/Import/Processors/Listing_Fetcher.php), [line 84](BigCommerce/Import/Processors/Listing_Fetcher.php#L84-L87)

Source: [src/BigCommerce/Import/Processors/Listing_Fetcher.php](BigCommerce/Import/Processors/Listing_Fetcher.php), [line 100](BigCommerce/Import/Processors/Listing_Fetcher.php#L100-L100)

Source: [src/BigCommerce/Import/Processors/Listing_Fetcher.php](BigCommerce/Import/Processors/Listing_Fetcher.php), [line 116](BigCommerce/Import/Processors/Listing_Fetcher.php#L116-L118)

Source: [src/BigCommerce/Import/Runner/AsyncProcessing_Runner.php](BigCommerce/Import/Runner/AsyncProcessing_Runner.php), [line 26](BigCommerce/Import/Runner/AsyncProcessing_Runner.php#L26-L28)

Source: [src/BigCommerce/Import/Runner/AsyncProcessing_Runner.php](BigCommerce/Import/Runner/AsyncProcessing_Runner.php), [line 34](BigCommerce/Import/Runner/AsyncProcessing_Runner.php#L34-L36)

Source: [src/BigCommerce/Import/Runner/Lock_Monitor.php](BigCommerce/Import/Runner/Lock_Monitor.php), [line 42](BigCommerce/Import/Runner/Lock_Monitor.php#L42-L44)

Source: [src/BigCommerce/Accounts/Customer.php](BigCommerce/Accounts/Customer.php), [line 426](BigCommerce/Accounts/Customer.php#L426-L433)

Source: [src/BigCommerce/Accounts/Register.php](BigCommerce/Accounts/Register.php), [line 94](BigCommerce/Accounts/Register.php#L94-L103)

Source: [src/BigCommerce/Accounts/Register.php](BigCommerce/Accounts/Register.php), [line 105](BigCommerce/Accounts/Register.php#L105-L114)

Source: [src/BigCommerce/Accounts/Register.php](BigCommerce/Accounts/Register.php), [line 163](BigCommerce/Accounts/Register.php#L163-L173)

Source: [src/BigCommerce/Accounts/Register.php](BigCommerce/Accounts/Register.php), [line 175](BigCommerce/Accounts/Register.php#L175-L184)

Source: [src/BigCommerce/Rest/Terms_Controller.php](BigCommerce/Rest/Terms_Controller.php), [line 82](BigCommerce/Rest/Terms_Controller.php#L82-L82)

Source: [src/BigCommerce/Rest/Terms_Controller.php](BigCommerce/Rest/Terms_Controller.php), [line 95](BigCommerce/Rest/Terms_Controller.php#L95-L95)

Source: [src/BigCommerce/Rest/Products_Controller.php](BigCommerce/Rest/Products_Controller.php), [line 145](BigCommerce/Rest/Products_Controller.php#L145-L145)

Source: [src/BigCommerce/Rest/Products_Controller.php](BigCommerce/Rest/Products_Controller.php), [line 264](BigCommerce/Rest/Products_Controller.php#L264-L264)

Source: [src/BigCommerce/Rest/Products_Controller.php](BigCommerce/Rest/Products_Controller.php), [line 330](BigCommerce/Rest/Products_Controller.php#L330-L332)

Source: [src/BigCommerce/Webhooks/Product/Channel_Updater.php](BigCommerce/Webhooks/Product/Channel_Updater.php), [line 14](BigCommerce/Webhooks/Product/Channel_Updater.php#L14-L16)

Source: [src/BigCommerce/Webhooks/Product/Channel_Updater.php](BigCommerce/Webhooks/Product/Channel_Updater.php), [line 25](BigCommerce/Webhooks/Product/Channel_Updater.php#L25-L27)

Source: [src/BigCommerce/Webhooks/Product/Channel_Updater.php](BigCommerce/Webhooks/Product/Channel_Updater.php), [line 51](BigCommerce/Webhooks/Product/Channel_Updater.php#L51-L54)

Source: [src/BigCommerce/Webhooks/Product/Channel_Updater.php](BigCommerce/Webhooks/Product/Channel_Updater.php), [line 59](BigCommerce/Webhooks/Product/Channel_Updater.php#L59-L62)

Source: [src/BigCommerce/Webhooks/Product/Product_Delete_Webhook.php](BigCommerce/Webhooks/Product/Product_Delete_Webhook.php), [line 30](BigCommerce/Webhooks/Product/Product_Delete_Webhook.php#L30-L37)

Source: [src/BigCommerce/Webhooks/Product/Channels_UnAssign.php](BigCommerce/Webhooks/Product/Channels_UnAssign.php), [line 17](BigCommerce/Webhooks/Product/Channels_UnAssign.php#L17-L19)

Source: [src/BigCommerce/Webhooks/Product/Channels_Management_Webhook.php](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php), [line 35](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php#L35-L37)

Source: [src/BigCommerce/Webhooks/Product/Channels_Management_Webhook.php](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php), [line 50](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php#L50-L53)

Source: [src/BigCommerce/Webhooks/Product/Channels_Management_Webhook.php](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php), [line 59](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php#L59-L62)

Source: [src/BigCommerce/Webhooks/Product/Channels_Management_Webhook.php](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php), [line 70](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php#L70-L74)

Source: [src/BigCommerce/Webhooks/Product/Product_Update_Webhook.php](BigCommerce/Webhooks/Product/Product_Update_Webhook.php), [line 30](BigCommerce/Webhooks/Product/Product_Update_Webhook.php#L30-L37)

Source: [src/BigCommerce/Webhooks/Product/Channels_Assign.php](BigCommerce/Webhooks/Product/Channels_Assign.php), [line 16](BigCommerce/Webhooks/Product/Channels_Assign.php#L16-L18)

Source: [src/BigCommerce/Webhooks/Product/Channels_Assign.php](BigCommerce/Webhooks/Product/Channels_Assign.php), [line 26](BigCommerce/Webhooks/Product/Channels_Assign.php#L26-L29)

Source: [src/BigCommerce/Webhooks/Product/Channels_Assign.php](BigCommerce/Webhooks/Product/Channels_Assign.php), [line 46](BigCommerce/Webhooks/Product/Channels_Assign.php#L46-L49)

Source: [src/BigCommerce/Webhooks/Product/Channels_Assign.php](BigCommerce/Webhooks/Product/Channels_Assign.php), [line 50](BigCommerce/Webhooks/Product/Channels_Assign.php#L50-L50)

Source: [src/BigCommerce/Webhooks/Product/Channels_Assign.php](BigCommerce/Webhooks/Product/Channels_Assign.php), [line 62](BigCommerce/Webhooks/Product/Channels_Assign.php#L62-L65)

Source: [src/BigCommerce/Webhooks/Product/Channels_Assign.php](BigCommerce/Webhooks/Product/Channels_Assign.php), [line 100](BigCommerce/Webhooks/Product/Channels_Assign.php#L100-L103)

Source: [src/BigCommerce/Webhooks/Product/Channels_Assign.php](BigCommerce/Webhooks/Product/Channels_Assign.php), [line 104](BigCommerce/Webhooks/Product/Channels_Assign.php#L104-L104)

Source: [src/BigCommerce/Webhooks/Product/Product_Create_Webhook.php](BigCommerce/Webhooks/Product/Product_Create_Webhook.php), [line 28](BigCommerce/Webhooks/Product/Product_Create_Webhook.php#L28-L35)

Source: [src/BigCommerce/Webhooks/Product/Channels_Currency_Update.php](BigCommerce/Webhooks/Product/Channels_Currency_Update.php), [line 22](BigCommerce/Webhooks/Product/Channels_Currency_Update.php#L22-L24)

Source: [src/BigCommerce/Webhooks/Product/Channels_Currency_Update.php](BigCommerce/Webhooks/Product/Channels_Currency_Update.php), [line 29](BigCommerce/Webhooks/Product/Channels_Currency_Update.php#L29-L31)

Source: [src/BigCommerce/Webhooks/Product/Channels_Currency_Update.php](BigCommerce/Webhooks/Product/Channels_Currency_Update.php), [line 42](BigCommerce/Webhooks/Product/Channels_Currency_Update.php#L42-L44)

Source: [src/BigCommerce/Webhooks/Product/Channels_Currency_Update.php](BigCommerce/Webhooks/Product/Channels_Currency_Update.php), [line 62](BigCommerce/Webhooks/Product/Channels_Currency_Update.php#L62-L67)

Source: [src/BigCommerce/Webhooks/Product/Channels_Currency_Update.php](BigCommerce/Webhooks/Product/Channels_Currency_Update.php), [line 93](BigCommerce/Webhooks/Product/Channels_Currency_Update.php#L93-L95)

Source: [src/BigCommerce/Webhooks/Product/Product_Inventory_Update_Webhook.php](BigCommerce/Webhooks/Product/Product_Inventory_Update_Webhook.php), [line 33](BigCommerce/Webhooks/Product/Product_Inventory_Update_Webhook.php#L33-L40)

Source: [src/BigCommerce/Webhooks/Product/Channels_Manager.php](BigCommerce/Webhooks/Product/Channels_Manager.php), [line 42](BigCommerce/Webhooks/Product/Channels_Manager.php#L42-L44)

Source: [src/BigCommerce/Webhooks/Product/Product_Creator.php](BigCommerce/Webhooks/Product/Product_Creator.php), [line 60](BigCommerce/Webhooks/Product/Product_Creator.php#L60-L60)

Source: [src/BigCommerce/Webhooks/Product/Product_Creator.php](BigCommerce/Webhooks/Product/Product_Creator.php), [line 105](BigCommerce/Webhooks/Product/Product_Creator.php#L105-L105)

Source: [src/BigCommerce/Webhooks/Product/Product_Creator.php](BigCommerce/Webhooks/Product/Product_Creator.php), [line 138](BigCommerce/Webhooks/Product/Product_Creator.php#L138-L138)

Source: [src/BigCommerce/Webhooks/Product/Product_Updater.php](BigCommerce/Webhooks/Product/Product_Updater.php), [line 115](BigCommerce/Webhooks/Product/Product_Updater.php#L115-L115)

Source: [src/BigCommerce/Webhooks/Webhook.php](BigCommerce/Webhooks/Webhook.php), [line 154](BigCommerce/Webhooks/Webhook.php#L154-L154)

Source: [src/BigCommerce/Webhooks/Webhook.php](BigCommerce/Webhooks/Webhook.php), [line 230](BigCommerce/Webhooks/Webhook.php#L230-L232)

Source: [src/BigCommerce/Webhooks/Webhook.php](BigCommerce/Webhooks/Webhook.php), [line 261](BigCommerce/Webhooks/Webhook.php#L261-L263)

Source: [src/BigCommerce/Webhooks/Customer/Customer_Creator.php](BigCommerce/Webhooks/Customer/Customer_Creator.php), [line 39](BigCommerce/Webhooks/Customer/Customer_Creator.php#L39-L42)

Source: [src/BigCommerce/Webhooks/Customer/Customer_Creator.php](BigCommerce/Webhooks/Customer/Customer_Creator.php), [line 52](BigCommerce/Webhooks/Customer/Customer_Creator.php#L52-L55)

Source: [src/BigCommerce/Webhooks/Customer/Customer_Channel_Updater.php](BigCommerce/Webhooks/Customer/Customer_Channel_Updater.php), [line 46](BigCommerce/Webhooks/Customer/Customer_Channel_Updater.php#L46-L48)

Source: [src/BigCommerce/Webhooks/Customer/Customer_Updater.php](BigCommerce/Webhooks/Customer/Customer_Updater.php), [line 30](BigCommerce/Webhooks/Customer/Customer_Updater.php#L30-L32)

Source: [src/BigCommerce/Webhooks/Customer/Customer_Update_Webhook.php](BigCommerce/Webhooks/Customer/Customer_Update_Webhook.php), [line 32](BigCommerce/Webhooks/Customer/Customer_Update_Webhook.php#L32-L39)

Source: [src/BigCommerce/Webhooks/Customer/Customer_Saver.php](BigCommerce/Webhooks/Customer/Customer_Saver.php), [line 40](BigCommerce/Webhooks/Customer/Customer_Saver.php#L40-L45)

Source: [src/BigCommerce/Webhooks/Customer/Customer_Saver.php](BigCommerce/Webhooks/Customer/Customer_Saver.php), [line 112](BigCommerce/Webhooks/Customer/Customer_Saver.php#L112-L114)

Source: [src/BigCommerce/Webhooks/Customer/Customer_Saver.php](BigCommerce/Webhooks/Customer/Customer_Saver.php), [line 123](BigCommerce/Webhooks/Customer/Customer_Saver.php#L123-L125)

Source: [src/BigCommerce/Webhooks/Customer/Customer_Saver.php](BigCommerce/Webhooks/Customer/Customer_Saver.php), [line 152](BigCommerce/Webhooks/Customer/Customer_Saver.php#L152-L155)

Source: [src/BigCommerce/Webhooks/Customer/Customer_Create_Webhook.php](BigCommerce/Webhooks/Customer/Customer_Create_Webhook.php), [line 29](BigCommerce/Webhooks/Customer/Customer_Create_Webhook.php#L29-L36)

Source: [src/BigCommerce/Webhooks/Customer/Customer_Channel_Webhook.php](BigCommerce/Webhooks/Customer/Customer_Channel_Webhook.php), [line 33](BigCommerce/Webhooks/Customer/Customer_Channel_Webhook.php#L33-L40)

Source: [src/BigCommerce/Webhooks/Customer/Customer_Delete_Webhook.php](BigCommerce/Webhooks/Customer/Customer_Delete_Webhook.php), [line 30](BigCommerce/Webhooks/Customer/Customer_Delete_Webhook.php#L30-L37)

Source: [src/BigCommerce/Settings/Import_Status.php](BigCommerce/Settings/Import_Status.php), [line 250](BigCommerce/Settings/Import_Status.php#L250-L252)

Source: [src/BigCommerce/Settings/Import_Status.php](BigCommerce/Settings/Import_Status.php), [line 253](BigCommerce/Settings/Import_Status.php#L253-L257)

Source: [src/BigCommerce/Settings/Abort_Import.php](BigCommerce/Settings/Abort_Import.php), [line 36](BigCommerce/Settings/Abort_Import.php#L36-L36)

Source: [src/BigCommerce/Post_Types/Product/Product.php](BigCommerce/Post_Types/Product/Product.php), [line 469](BigCommerce/Post_Types/Product/Product.php#L469-L469)

Source: [src/BigCommerce/Taxonomies/Channel/Channel_Synchronizer.php](BigCommerce/Taxonomies/Channel/Channel_Synchronizer.php), [line 65](BigCommerce/Taxonomies/Channel/Channel_Synchronizer.php#L65-L70)

Source: [src/BigCommerce/Taxonomies/Channel/Channel_Synchronizer.php](BigCommerce/Taxonomies/Channel/Channel_Synchronizer.php), [line 71](BigCommerce/Taxonomies/Channel/Channel_Synchronizer.php#L71-L71)

Source: [src/BigCommerce/Taxonomies/Channel/Channel_Synchronizer.php](BigCommerce/Taxonomies/Channel/Channel_Synchronizer.php), [line 85](BigCommerce/Taxonomies/Channel/Channel_Synchronizer.php#L85-L85)

Source: [src/BigCommerce/Taxonomies/Channel/Channel_Synchronizer.php](BigCommerce/Taxonomies/Channel/Channel_Synchronizer.php), [line 86](BigCommerce/Taxonomies/Channel/Channel_Synchronizer.php#L86-L86)

Source: [src/BigCommerce/Taxonomies/Channel/Channel_Synchronizer.php](BigCommerce/Taxonomies/Channel/Channel_Synchronizer.php), [line 184](BigCommerce/Taxonomies/Channel/Channel_Synchronizer.php#L184-L184)

Source: [src/BigCommerce/Taxonomies/Channel/Connections.php](BigCommerce/Taxonomies/Channel/Connections.php), [line 106](BigCommerce/Taxonomies/Channel/Connections.php#L106-L109)

Source: [src/BigCommerce/Manager/Manager.php](BigCommerce/Manager/Manager.php), [line 29](BigCommerce/Manager/Manager.php#L29-L29)

Source: [src/BigCommerce/Manager/Manager.php](BigCommerce/Manager/Manager.php), [line 36](BigCommerce/Manager/Manager.php#L36-L38)

Source: [src/BigCommerce/Manager/Manager.php](BigCommerce/Manager/Manager.php), [line 48](BigCommerce/Manager/Manager.php#L48-L50)

Source: [src/BigCommerce/Manager/Manager.php](BigCommerce/Manager/Manager.php), [line 55](BigCommerce/Manager/Manager.php#L55-L57)

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 633](BigCommerce/Container/Import.php#L633-L633)

Source: [src/BigCommerce/Api/Api_Scopes_Validator.php](BigCommerce/Api/Api_Scopes_Validator.php), [line 90](BigCommerce/Api/Api_Scopes_Validator.php#L90-L99)

Source: [src/BigCommerce/Api/Api_Scopes_Validator.php](BigCommerce/Api/Api_Scopes_Validator.php), [line 115](BigCommerce/Api/Api_Scopes_Validator.php#L115-L124)

### login_form

Source: [src/BigCommerce/Templates/Login_Form.php](BigCommerce/Templates/Login_Form.php), [line 39](BigCommerce/Templates/Login_Form.php#L39-L39)

### bigcommerce/import/marked_deleted


Triggered when a batch of posts have been marked for deletion, due
to removal from the BigCommerce store, or the disconnection of a channel

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`count` | `int` | The number of deletions added to the queue
`posts_to_delete` | `int[]` | The IDs of the posts that will be deleted

Source: [src/BigCommerce/Import/Processors/Deleted_Product_Marker.php](BigCommerce/Import/Processors/Deleted_Product_Marker.php), [line 102](BigCommerce/Import/Processors/Deleted_Product_Marker.php#L102-L109)

### bigcommerce/import/error


Action to log import errors during the BigCommerce import process.

This action is triggered when there is an error during the import process. It logs the error message and context for further analysis.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`message` | `string` | The error message to be logged.
`context` | `array` | Additional context for the error.

Source: [src/BigCommerce/Import/Processors/Term_Purge.php](BigCommerce/Import/Processors/Term_Purge.php), [line 84](BigCommerce/Import/Processors/Term_Purge.php#L84-L95)

Source: [src/BigCommerce/Import/Processors/Headless_Product_Processor.php](BigCommerce/Import/Processors/Headless_Product_Processor.php), [line 132](BigCommerce/Import/Processors/Headless_Product_Processor.php#L132-L135)

Source: [src/BigCommerce/Import/Processors/Category_Import.php](BigCommerce/Import/Processors/Category_Import.php), [line 116](BigCommerce/Import/Processors/Category_Import.php#L116-L119)

Source: [src/BigCommerce/Import/Processors/Channel_Initializer.php](BigCommerce/Import/Processors/Channel_Initializer.php), [line 128](BigCommerce/Import/Processors/Channel_Initializer.php#L128-L128)

Source: [src/BigCommerce/Import/Processors/Channel_Initializer.php](BigCommerce/Import/Processors/Channel_Initializer.php), [line 142](BigCommerce/Import/Processors/Channel_Initializer.php#L142-L145)

Source: [src/BigCommerce/Import/Processors/Channel_Initializer.php](BigCommerce/Import/Processors/Channel_Initializer.php), [line 177](BigCommerce/Import/Processors/Channel_Initializer.php#L177-L180)

Source: [src/BigCommerce/Import/Processors/Channel_Initializer.php](BigCommerce/Import/Processors/Channel_Initializer.php), [line 246](BigCommerce/Import/Processors/Channel_Initializer.php#L246-L249)

Source: [src/BigCommerce/Import/Processors/Listing_Fetcher.php](BigCommerce/Import/Processors/Listing_Fetcher.php), [line 57](BigCommerce/Import/Processors/Listing_Fetcher.php#L57-L57)

Source: [src/BigCommerce/Import/Processors/Listing_Fetcher.php](BigCommerce/Import/Processors/Listing_Fetcher.php), [line 96](BigCommerce/Import/Processors/Listing_Fetcher.php#L96-L99)

Source: [src/BigCommerce/Webhooks/Product/Product_Creator.php](BigCommerce/Webhooks/Product/Product_Creator.php), [line 59](BigCommerce/Webhooks/Product/Product_Creator.php#L59-L59)

Source: [src/BigCommerce/Webhooks/Product/Product_Creator.php](BigCommerce/Webhooks/Product/Product_Creator.php), [line 101](BigCommerce/Webhooks/Product/Product_Creator.php#L101-L104)

Source: [src/BigCommerce/Webhooks/Product/Product_Creator.php](BigCommerce/Webhooks/Product/Product_Creator.php), [line 134](BigCommerce/Webhooks/Product/Product_Creator.php#L134-L137)

Source: [src/BigCommerce/Webhooks/Product/Product_Updater.php](BigCommerce/Webhooks/Product/Product_Updater.php), [line 68](BigCommerce/Webhooks/Product/Product_Updater.php#L68-L68)

Source: [src/BigCommerce/Webhooks/Product/Product_Updater.php](BigCommerce/Webhooks/Product/Product_Updater.php), [line 111](BigCommerce/Webhooks/Product/Product_Updater.php#L111-L114)

Source: [src/BigCommerce/Taxonomies/Channel/BC_Status.php](BigCommerce/Taxonomies/Channel/BC_Status.php), [line 29](BigCommerce/Taxonomies/Channel/BC_Status.php#L29-L29)

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 632](BigCommerce/Container/Import.php#L632-L632)

### bigcommerce/import/fetched_currency


Hook after fetching currency code.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`currency_code` | `string` | The fetched currency code.

Source: [src/BigCommerce/Import/Processors/Store_Settings.php](BigCommerce/Import/Processors/Store_Settings.php), [line 116](BigCommerce/Import/Processors/Store_Settings.php#L116-L121)

### bigcommerce/import/fetched_store_settings


Checks and updates routes after fetching store settings during an import.

Triggers the `maybe_update_routes` method of the `Routes` class to ensure routes are updated
after store settings are fetched during the import process.

**Arguments**

No arguments.

Source: [src/BigCommerce/Import/Processors/Store_Settings.php](BigCommerce/Import/Processors/Store_Settings.php), [line 122](BigCommerce/Import/Processors/Store_Settings.php#L122-L128)

### bigcommerce/import/could_not_fetch_store_settings


Hook when store settings cannot be fetched.

**Arguments**

No arguments.

Source: [src/BigCommerce/Import/Processors/Store_Settings.php](BigCommerce/Import/Processors/Store_Settings.php), [line 131](BigCommerce/Import/Processors/Store_Settings.php#L131-L134)

### bigcommerce/import/fetched_products


Triggered when a batch of products have been fetched from the BigCommerce
API and stored in the import queue

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`count` | `int` | The number of products added to the queue
`api_response` | `\BigCommerce\Api\v3\Model\ProductCollectionResponse` | The response received from the BigCommerce API

Source: [src/BigCommerce/Import/Processors/Product_Data_Fetcher.php](BigCommerce/Import/Processors/Product_Data_Fetcher.php), [line 168](BigCommerce/Import/Processors/Product_Data_Fetcher.php#L168-L175)

### bigcommerce/import/fetched_currencies

Source: [src/BigCommerce/Import/Processors/Currencies.php](BigCommerce/Import/Processors/Currencies.php), [line 83](BigCommerce/Import/Processors/Currencies.php#L83-L83)

### bigcommerce/import/could_not_fetch_currency_settings

Source: [src/BigCommerce/Import/Processors/Currencies.php](BigCommerce/Import/Processors/Currencies.php), [line 85](BigCommerce/Import/Processors/Currencies.php#L85-L85)

### Cron_Runner::START_CRON


Begins the import process when the `Runner\Cron_Runner::START_CRON` action is triggered.

**Arguments**

No arguments.

Source: [src/BigCommerce/Import/Processors/Headless.php](BigCommerce/Import/Processors/Headless.php), [line 28](BigCommerce/Import/Processors/Headless.php#L28-L33)

Source: [src/BigCommerce/Settings/Import_Now.php](BigCommerce/Settings/Import_Now.php), [line 144](BigCommerce/Settings/Import_Now.php#L144-L144)

### bigcommerce/import/log


Action to log messages during the BigCommerce logging process.

This action is triggered when a log entry needs to be created. It logs the message, context, level, and path to the log file.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`level` | `string` | The log level (e.g., INFO, ERROR).
`message` | `string` | The log message to be recorded.
`context` | `array` | Additional context for the log entry.
`path` | `string` | The path where the log is being written.

Source: [src/BigCommerce/Import/Image_Importer.php](BigCommerce/Import/Image_Importer.php), [line 68](BigCommerce/Import/Image_Importer.php#L68-L82)

Source: [src/BigCommerce/Import/Image_Importer.php](BigCommerce/Import/Image_Importer.php), [line 100](BigCommerce/Import/Image_Importer.php#L100-L103)

Source: [src/BigCommerce/Import/Image_Importer.php](BigCommerce/Import/Image_Importer.php), [line 191](BigCommerce/Import/Image_Importer.php#L191-L194)

Source: [src/BigCommerce/Import/Image_Importer.php](BigCommerce/Import/Image_Importer.php), [line 219](BigCommerce/Import/Image_Importer.php#L219-L222)

Source: [src/BigCommerce/Import/Importers/Terms/Term_Updater.php](BigCommerce/Import/Importers/Terms/Term_Updater.php), [line 29](BigCommerce/Import/Importers/Terms/Term_Updater.php#L29-L32)

Source: [src/BigCommerce/Import/Importers/Terms/Term_Creator.php](BigCommerce/Import/Importers/Terms/Term_Creator.php), [line 29](BigCommerce/Import/Importers/Terms/Term_Creator.php#L29-L42)

Source: [src/BigCommerce/Post_Types/Product/Product.php](BigCommerce/Post_Types/Product/Product.php), [line 465](BigCommerce/Post_Types/Product/Product.php#L465-L468)

### bigcommerce/import/product/skipped


Fires when a product is skipped during the import process.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_id` | `int` | The WordPress post ID of the skipped product.
`product` | `\BigCommerce\Api\v3\Model\Product` | The product data from the BigCommerce API.
`listing` | `\BigCommerce\Api\v3\Model\Listing` | The channel listing data.
`channel_term` | `\WP_Term` | The term representing the product's channel.
`catalog` | `\BigCommerce\Api\v3\Api\CatalogApi` | The Catalog API instance used for product operations.

Source: [src/BigCommerce/Import/Importers/Products/Product_Ignorer.php](BigCommerce/Import/Importers/Products/Product_Ignorer.php), [line 67](BigCommerce/Import/Importers/Products/Product_Ignorer.php#L67-L76)

### bigcommerce/import/product/saved


A product has been saved by the import process

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_id` | `int` | The Post ID of the skipped product
`product` | `\BigCommerce\Api\v3\Model\Product` | The product data
`listing` | `\BigCommerce\Api\v3\Model\Listing` | The channel listing data
`catalog` | `\BigCommerce\Api\v3\Api\CatalogApi` | The Catalog API instance

Source: [src/BigCommerce/Import/Importers/Products/Product_Saver.php](BigCommerce/Import/Importers/Products/Product_Saver.php), [line 235](BigCommerce/Import/Importers/Products/Product_Saver.php#L235-L243)

### bigcommerce/import/product/created


Fires after a product has been created during the import process.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_id` | `int` | The WordPress post ID of the created product.
`product` | `\BigCommerce\Api\v3\Model\Product` | The product data from the BigCommerce API.
`listing` | `\BigCommerce\Api\v3\Model\Listing` | The channel listing data from the BigCommerce API.
`catalog` | `\BigCommerce\Api\v3\Api\CatalogApi` | The Catalog API instance used for the import.

Source: [src/BigCommerce/Import/Importers/Products/Product_Creator.php](BigCommerce/Import/Importers/Products/Product_Creator.php), [line 58](BigCommerce/Import/Importers/Products/Product_Creator.php#L58-L66)

### bigcommerce/import/product/updated


A product has been updated by the import process

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_id` | `int` | The Post ID of the updated product
`product` | `\BigCommerce\Api\v3\Model\Product` | The product data
`listing` | `\BigCommerce\Api\v3\Model\Listing` | The channel listing data
`catalog` | `\BigCommerce\Api\v3\Api\CatalogApi` | The Catalog API instance

Source: [src/BigCommerce/Import/Importers/Products/Product_Updater.php](BigCommerce/Import/Importers/Products/Product_Updater.php), [line 24](BigCommerce/Import/Importers/Products/Product_Updater.php#L24-L32)

### bigcommerce/import/term/skipped


A term has been skipped for import.

This action is triggered when a term is skipped for import. It allows other functions to react
to the skipping of the term.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`bc_term` | `array` | The BigCommerce term data.
`taxonomy` | `string` | The taxonomy of the term.
`term_id` | `int` | The term ID in WordPress.

Source: [src/BigCommerce/Import/Importers/Terms/Term_Ignorer.php](BigCommerce/Import/Importers/Terms/Term_Ignorer.php), [line 53](BigCommerce/Import/Importers/Terms/Term_Ignorer.php#L53-L63)

### bigcommerce/import/start


This action is triggered at the start of the BigCommerce import process. It clears or truncates the log file to ensure that old logs do not interfere with the new import process.

**Arguments**

No arguments.

Source: [src/BigCommerce/Import/Runner/Cron_Runner.php](BigCommerce/Import/Runner/Cron_Runner.php), [line 30](BigCommerce/Import/Runner/Cron_Runner.php#L30-L33)

Source: [src/BigCommerce/Import/Runner/CLI_Runner.php](BigCommerce/Import/Runner/CLI_Runner.php), [line 22](BigCommerce/Import/Runner/CLI_Runner.php#L22-L22)

### bigcommerce/import/before


Hook before the import starts.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`status` | `string` | Current status of the import.

Source: [src/BigCommerce/Import/Runner/Cron_Runner.php](BigCommerce/Import/Runner/Cron_Runner.php), [line 55](BigCommerce/Import/Runner/Cron_Runner.php#L55-L60)

Source: [src/BigCommerce/Import/Runner/AsyncProcessing_Runner.php](BigCommerce/Import/Runner/AsyncProcessing_Runner.php), [line 43](BigCommerce/Import/Runner/AsyncProcessing_Runner.php#L43-L43)

Source: [src/BigCommerce/Import/Runner/CLI_Runner.php](BigCommerce/Import/Runner/CLI_Runner.php), [line 29](BigCommerce/Import/Runner/CLI_Runner.php#L29-L29)

### bigcommerce/import/run


Hook to run the import process.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`status` | `string` | Current status of the import.

Source: [src/BigCommerce/Import/Runner/Cron_Runner.php](BigCommerce/Import/Runner/Cron_Runner.php), [line 61](BigCommerce/Import/Runner/Cron_Runner.php#L61-L66)

Source: [src/BigCommerce/Import/Runner/AsyncProcessing_Runner.php](BigCommerce/Import/Runner/AsyncProcessing_Runner.php), [line 44](BigCommerce/Import/Runner/AsyncProcessing_Runner.php#L44-L44)

Source: [src/BigCommerce/Import/Runner/CLI_Runner.php](BigCommerce/Import/Runner/CLI_Runner.php), [line 30](BigCommerce/Import/Runner/CLI_Runner.php#L30-L30)

### bigcommerce/import/after


Hook after the import finishes.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`status` | `string` | Current status of the import.

Source: [src/BigCommerce/Import/Runner/Cron_Runner.php](BigCommerce/Import/Runner/Cron_Runner.php), [line 67](BigCommerce/Import/Runner/Cron_Runner.php#L67-L72)

Source: [src/BigCommerce/Import/Runner/AsyncProcessing_Runner.php](BigCommerce/Import/Runner/AsyncProcessing_Runner.php), [line 45](BigCommerce/Import/Runner/AsyncProcessing_Runner.php#L45-L45)

Source: [src/BigCommerce/Import/Runner/CLI_Runner.php](BigCommerce/Import/Runner/CLI_Runner.php), [line 31](BigCommerce/Import/Runner/CLI_Runner.php#L31-L31)

### self::CONTINUE_CRON

Source: [src/BigCommerce/Import/Runner/Cron_Runner.php](BigCommerce/Import/Runner/Cron_Runner.php), [line 93](BigCommerce/Import/Runner/Cron_Runner.php#L93-L93)

### bigcommerce/import/set_status


Hook when the import status is set.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`status` | `string` | The status being set.

Source: [src/BigCommerce/Import/Runner/Status.php](BigCommerce/Import/Runner/Status.php), [line 76](BigCommerce/Import/Runner/Status.php#L76-L81)

### bigcommerce/import/logs/rotate


Rotate out the current log into the previous log slot

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`log` | `array` | The current log

Source: [src/BigCommerce/Import/Runner/Status.php](BigCommerce/Import/Runner/Status.php), [line 91](BigCommerce/Import/Runner/Status.php#L91-L96)

### bigcommerce/import/logs/rotated


Logs have been rotated

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`log` | `array` | The previous log

Source: [src/BigCommerce/Import/Runner/Status.php](BigCommerce/Import/Runner/Status.php), [line 99](BigCommerce/Import/Runner/Status.php#L99-L104)

### bigcommerce/wishlist_endpoint/{$action}


Routes the request to the appropriate wishlist action handler.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`action` | `string` | The wishlist action to be executed
`args` | `array` | The arguments for the wishlist request

Source: [src/BigCommerce/Accounts/Wishlists/Actions/Request_Router.php](BigCommerce/Accounts/Wishlists/Actions/Request_Router.php), [line 39](BigCommerce/Accounts/Wishlists/Actions/Request_Router.php#L39-L45)

### bigcommerce/table_maker/created_table

Source: [src/BigCommerce/Schema/Table_Maker.php](BigCommerce/Schema/Table_Maker.php), [line 66](BigCommerce/Schema/Table_Maker.php#L66-L66)

### bigcommerce/webhooks/product_deleted

Source: [src/BigCommerce/Webhooks/Product/Product_Delete_Webhook.php](BigCommerce/Webhooks/Product/Product_Delete_Webhook.php), [line 38](BigCommerce/Webhooks/Product/Product_Delete_Webhook.php#L38-L38)

### self::CHANNEL_UPDATED_HOOK

Source: [src/BigCommerce/Webhooks/Product/Channels_Management_Webhook.php](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php), [line 48](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php#L48-L48)

### self::CHANNEL_CURRENCY_UPDATE_HOOK

Source: [src/BigCommerce/Webhooks/Product/Channels_Management_Webhook.php](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php), [line 84](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php#L84-L84)

### sprintf()

Source: [src/BigCommerce/Webhooks/Product/Channels_Management_Webhook.php](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php), [line 90](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php#L90-L90)

Source: [src/BigCommerce/Webhooks/Product/Channels_Management_Webhook.php](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php), [line 95](BigCommerce/Webhooks/Product/Channels_Management_Webhook.php#L95-L95)

### bigcommerce/webhooks/product_updated


Handles the "product updated" webhook event.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`params` | `array` | The parameters of the updated product, including product ID.

Source: [src/BigCommerce/Webhooks/Product/Product_Update_Webhook.php](BigCommerce/Webhooks/Product/Product_Update_Webhook.php), [line 38](BigCommerce/Webhooks/Product/Product_Update_Webhook.php#L38-L43)

### bigcommerce/import/update_product/skipped


Fires if product update import skipped.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`message` | `string` | Message.
`product_bc_id` | `int` | Product BC ID.

Source: [src/BigCommerce/Webhooks/Product/Channels_Assign.php](BigCommerce/Webhooks/Product/Channels_Assign.php), [line 82](BigCommerce/Webhooks/Product/Channels_Assign.php#L82-L88)

Source: [src/BigCommerce/Webhooks/Product/Product_Updater.php](BigCommerce/Webhooks/Product/Product_Updater.php), [line 139](BigCommerce/Webhooks/Product/Product_Updater.php#L139-L145)

### bigcommerce/webhooks/product_created

Source: [src/BigCommerce/Webhooks/Product/Product_Create_Webhook.php](BigCommerce/Webhooks/Product/Product_Create_Webhook.php), [line 36](BigCommerce/Webhooks/Product/Product_Create_Webhook.php#L36-L36)

### bigcommerce/webhooks/product_inventory_updated


Handles the "product inventory updated" webhook event.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`params` | `array` | Parameters for the updated product, including product ID.

Source: [src/BigCommerce/Webhooks/Product/Product_Inventory_Update_Webhook.php](BigCommerce/Webhooks/Product/Product_Inventory_Update_Webhook.php), [line 41](BigCommerce/Webhooks/Product/Product_Inventory_Update_Webhook.php#L41-L46)

### bigcommerce/webhooks/webhook_updated


Fires when a webhook is added to the BigCommerce database.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`` | `int` | Webhook ID.
`` | `string` | Webhook action name.
`` | `string` | Webhook scope.

Source: [src/BigCommerce/Webhooks/Webhook.php](BigCommerce/Webhooks/Webhook.php), [line 172](BigCommerce/Webhooks/Webhook.php#L172-L179)

Source: [src/BigCommerce/Webhooks/Webhook.php](BigCommerce/Webhooks/Webhook.php), [line 126](BigCommerce/Webhooks/Webhook.php#L126-L126)

### bigcommerce/webhooks/update_failed


Fires after webhook update failed.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`` | `\BigCommerce\Webhooks\Webhook` | Webhook Webhook class.
`result` | `array` | Result.

Source: [src/BigCommerce/Webhooks/Webhook.php](BigCommerce/Webhooks/Webhook.php), [line 146](BigCommerce/Webhooks/Webhook.php#L146-L152)

### bigcommerce/webhooks/delete_failed


Fires after webhook delete failed.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`` | `\BigCommerce\Webhooks\Webhook` | Webhook Webhook class.
`result` | `array` | Result.

Source: [src/BigCommerce/Webhooks/Webhook.php](BigCommerce/Webhooks/Webhook.php), [line 222](BigCommerce/Webhooks/Webhook.php#L222-L228)

### bigcommerce/webhooks/webhook_deleted


Fires when a webhook is deleted from the BigCommerce database.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`` | `int` | Webhook ID.
`` | `string` | Webhook action name.
`` | `string` | Webhook scope.

Source: [src/BigCommerce/Webhooks/Webhook.php](BigCommerce/Webhooks/Webhook.php), [line 235](BigCommerce/Webhooks/Webhook.php#L235-L242)

### bigcommerce/webhooks/self::NAME


Fires when a product inventory webhooks has been received from the BigCommerce store.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`product_id` | `int` | BigCommerce product ID.

Source: [src/BigCommerce/Webhooks/Checkout_Complete_Webhook.php](BigCommerce/Webhooks/Checkout_Complete_Webhook.php), [line 28](BigCommerce/Webhooks/Checkout_Complete_Webhook.php#L28-L33)

### bigcommerce/settings/webhoooks_updated


This hook is documented in src/BigCommerce/Webhooks/Webhook.php.

**Arguments**

No arguments.

Source: [src/BigCommerce/Webhooks/Status.php](BigCommerce/Webhooks/Status.php), [line 107](BigCommerce/Webhooks/Status.php#L107-L110)

### bigcommerce/webhooks/customer_updated

Source: [src/BigCommerce/Webhooks/Customer/Customer_Update_Webhook.php](BigCommerce/Webhooks/Customer/Customer_Update_Webhook.php), [line 40](BigCommerce/Webhooks/Customer/Customer_Update_Webhook.php#L40-L40)

### bigcommerce/webhooks/customer_created

Source: [src/BigCommerce/Webhooks/Customer/Customer_Create_Webhook.php](BigCommerce/Webhooks/Customer/Customer_Create_Webhook.php), [line 37](BigCommerce/Webhooks/Customer/Customer_Create_Webhook.php#L37-L37)

### self::HOOK

Source: [src/BigCommerce/Webhooks/Customer/Customer_Channel_Webhook.php](BigCommerce/Webhooks/Customer/Customer_Channel_Webhook.php), [line 42](BigCommerce/Webhooks/Customer/Customer_Channel_Webhook.php#L42-L42)

### bigcommerce/webhooks/customer_deleted

Source: [src/BigCommerce/Webhooks/Customer/Customer_Delete_Webhook.php](BigCommerce/Webhooks/Customer/Customer_Delete_Webhook.php), [line 38](BigCommerce/Webhooks/Customer/Customer_Delete_Webhook.php#L38-L38)

### bigcommerce/settings/import/product_list_table_notice


Displays the current import status notice in the product list table.

**Arguments**

No arguments.

Source: [src/BigCommerce/Settings/Import_Now.php](BigCommerce/Settings/Import_Now.php), [line 177](BigCommerce/Settings/Import_Now.php#L177-L180)

### bigcommerce/settings/before_title/page=static::NAME

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 133](BigCommerce/Settings/Screens/Abstract_Screen.php#L133-L133)

### bigcommerce/settings/register/screen=static::NAME


Triggered after registering a settings screen. The dynamic
portion of the hook is the name of the screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`hook_suffix` | `string` | The hook suffix generated for the screen
`name` | `string` | The name of the screen

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 187](BigCommerce/Settings/Screens/Abstract_Screen.php#L187-L194)

### bigcommerce/settings/after_start_form/page=static::NAME


Triggered after the opening <form> tag on the settings screen form finishes rendering.

The dynamic portion of the hook is the identifier of the settings screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`hook_suffix` | `string` | The hook suffix generated for the screen

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 254](BigCommerce/Settings/Screens/Abstract_Screen.php#L254-L260)

### bigcommerce/settings/before_end_form/page=static::NAME


Triggered before the closing </form> tag on the settings screen form finishes rendering.

The dynamic portion of the hook is the identifier of the settings screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`hook_suffix` | `string` | The hook suffix generated for the screen

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 269](BigCommerce/Settings/Screens/Abstract_Screen.php#L269-L275)

### bigcommerce/settings/before_form/page=static::NAME


Triggered before the settings screen form starts to render.

The dynamic portion of the hook is the identifier of the settings screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`hook_suffix` | `string` | The hook suffix generated for the screen

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 314](BigCommerce/Settings/Screens/Abstract_Screen.php#L314-L320)

### bigcommerce/settings/after_form/page=static::NAME


Triggered after the settings screen form finishes rendering.

The dynamic portion of the hook is the identifier of the settings screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`hook_suffix` | `string` | The hook suffix generated for the screen

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 329](BigCommerce/Settings/Screens/Abstract_Screen.php#L329-L335)

### bigcommerce/settings/section/before/id={$section}[id]


Fires before rendering a settings section.

The dynamic portion of the hook name is the section ID.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`section` | `array` | 

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 354](BigCommerce/Settings/Screens/Abstract_Screen.php#L354-L360)

### bigcommerce/settings/section/after/id={$section}[id]


Fires after rendering a settings section.

The dynamic portion of the hook name is the section ID.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`section` | `array` | 

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 370](BigCommerce/Settings/Screens/Abstract_Screen.php#L370-L376)

### bigcommerce/settings/section/before_title/id={$section}[id]


Fires before rendering the title of a settings section.

The dynamic portion of the hook name is the section ID.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`section` | `array` | 

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 391](BigCommerce/Settings/Screens/Abstract_Screen.php#L391-L397)

### bigcommerce/settings/section/after_title/id={$section}[id]


Fires after rendering the title of a settings section.

The dynamic portion of the hook name is the section ID.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`section` | `array` | 

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 403](BigCommerce/Settings/Screens/Abstract_Screen.php#L403-L409)

### bigcommerce/settings/section/before_callback/id={$section}[id]


Fires before calling the callback of a settings section.

The dynamic portion of the hook name is the section ID.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`section` | `array` | 

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 427](BigCommerce/Settings/Screens/Abstract_Screen.php#L427-L433)

### bigcommerce/settings/section/after_callback/id={$section}[id]


Fires after calling the callback of a settings section.

The dynamic portion of the hook name is the section ID.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`section` | `array` | 

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 439](BigCommerce/Settings/Screens/Abstract_Screen.php#L439-L445)

### bigcommerce/settings/section/before_fields/id={$section}[id]


Fires before rendering the fields of a settings section.

The dynamic portion of the hook name is the section ID.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`section` | `array` | 
`has_fields` | `bool` | Whether the settings section has any fields to render

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 449](BigCommerce/Settings/Screens/Abstract_Screen.php#L449-L456)

### bigcommerce/settings/section/after_fields/id={$section}[id]


Fires after rendering the fields of a settings section.

The dynamic portion of the hook name is the section ID.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`section` | `array` | 
`has_fields` | `bool` | Whether the settings section has any fields to render

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 464](BigCommerce/Settings/Screens/Abstract_Screen.php#L464-L471)

### bigcommerce/settings/unregistered_screen


Redirects to the appropriate screen when an unregistered screen is encountered.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`unregistered_screen` | `string` | The name of the unregistered screen.

Source: [src/BigCommerce/Settings/Screens/Abstract_Screen.php](BigCommerce/Settings/Screens/Abstract_Screen.php), [line 500](BigCommerce/Settings/Screens/Abstract_Screen.php#L500-L505)

### bigcommerce/settings/onboarding/progress


Registers a callback to render the onboarding progress bar on the 'bigcommerce/settings/onboarding/progress' hook.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`progress_bar` | `callable` | The callback function to render the progress bar.
`priority` | `int` | The priority at which the callback should be executed. Defaults to 10.
`accepted_args` | `int` | The number of arguments the callback accepts. Defaults to 0.

Source: [src/BigCommerce/Settings/Screens/Onboarding_Screen.php](BigCommerce/Settings/Screens/Onboarding_Screen.php), [line 18](BigCommerce/Settings/Screens/Onboarding_Screen.php#L18-L25)

### bigcommerce/settings/after_content/page=static::NAME


Triggered before the settings screen form starts to render.

The dynamic portion of the hook is the identifier of the settings screen.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`hook_suffix` | `string` | The hook suffix generated for the screen

Source: [src/BigCommerce/Settings/Screens/Pending_Account_Screen.php](BigCommerce/Settings/Screens/Pending_Account_Screen.php), [line 47](BigCommerce/Settings/Screens/Pending_Account_Screen.php#L47-L53)

### bigcommerce/create_account/validate_request


Validates the request for creating a new BigCommerce account.

This action is triggered when a request is made to create a new account. It validates
the submission data and checks for any errors before processing the request.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`submission` | `array` | The submitted data from the account creation form.
`errors` | `array` | The array of validation errors, if any.

Source: [src/BigCommerce/Settings/Screens/Create_Account_Screen.php](BigCommerce/Settings/Screens/Create_Account_Screen.php), [line 79](BigCommerce/Settings/Screens/Create_Account_Screen.php#L79-L89)

### bigcommerce/create_account/submit_request


Action to handle the submission of account creation requests.

This action processes data submitted for account creation, logs errors,
and invokes the Create_Account service to handle the request.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | Submitted data for account creation.
`errors` | `array` | An array of errors, if any, encountered during submission.

Source: [src/BigCommerce/Settings/Screens/Create_Account_Screen.php](BigCommerce/Settings/Screens/Create_Account_Screen.php), [line 92](BigCommerce/Settings/Screens/Create_Account_Screen.php#L92-L103)

### bigcommerce/settings/header/import_status


Triggered after rendering the last import date in the settings header

**Arguments**

No arguments.

Source: [src/BigCommerce/Settings/Screens/Settings_Screen.php](BigCommerce/Settings/Screens/Settings_Screen.php), [line 64](BigCommerce/Settings/Screens/Settings_Screen.php#L64-L67)

### bigcommerce/settings/render/channel_select

Source: [src/BigCommerce/Settings/Sections/Channel_Select.php](BigCommerce/Settings/Sections/Channel_Select.php), [line 71](BigCommerce/Settings/Sections/Channel_Select.php#L71-L71)

### bigcommerce/settings/render/gift_certificates

Source: [src/BigCommerce/Settings/Sections/Gift_Certificates.php](BigCommerce/Settings/Sections/Gift_Certificates.php), [line 34](BigCommerce/Settings/Sections/Gift_Certificates.php#L34-L34)

### bigcommerce/settings/render/nav_menu_options/top

Source: [src/BigCommerce/Settings/Sections/Nav_Menu_Options.php](BigCommerce/Settings/Sections/Nav_Menu_Options.php), [line 25](BigCommerce/Settings/Sections/Nav_Menu_Options.php#L25-L25)

### bigcommerce/settings/accounts/before_page_field

Source: [src/BigCommerce/Settings/Sections/WithPages.php](BigCommerce/Settings/Sections/WithPages.php), [line 17](BigCommerce/Settings/Sections/WithPages.php#L17-L17)

### bigcommerce/settings/accounts/before_page_field/page={$option}

Source: [src/BigCommerce/Settings/Sections/WithPages.php](BigCommerce/Settings/Sections/WithPages.php), [line 18](BigCommerce/Settings/Sections/WithPages.php#L18-L18)

### bigcommerce/settings/accounts/after_page_field

Source: [src/BigCommerce/Settings/Sections/WithPages.php](BigCommerce/Settings/Sections/WithPages.php), [line 38](BigCommerce/Settings/Sections/WithPages.php#L38-L38)

### bigcommerce/settings/accounts/after_page_field/page={$option}

Source: [src/BigCommerce/Settings/Sections/WithPages.php](BigCommerce/Settings/Sections/WithPages.php), [line 39](BigCommerce/Settings/Sections/WithPages.php#L39-L39)

### bigcommerce/settings/render/cart

Source: [src/BigCommerce/Settings/Sections/Cart.php](BigCommerce/Settings/Sections/Cart.php), [line 149](BigCommerce/Settings/Sections/Cart.php#L149-L149)

### bigcommerce/settings/render/accounts

Source: [src/BigCommerce/Settings/Sections/Account_Settings.php](BigCommerce/Settings/Sections/Account_Settings.php), [line 37](BigCommerce/Settings/Sections/Account_Settings.php#L37-L37)

### bigcommerce/sync_global_logins


Sync global logins with BigCommerce

**Arguments**

No arguments.

Source: [src/BigCommerce/Settings/Sections/Account_Settings.php](BigCommerce/Settings/Sections/Account_Settings.php), [line 149](BigCommerce/Settings/Sections/Account_Settings.php#L149-L150)

### bigcommerce/settings/render/analytics

Source: [src/BigCommerce/Settings/Sections/Analytics.php](BigCommerce/Settings/Sections/Analytics.php), [line 50](BigCommerce/Settings/Sections/Analytics.php#L50-L50)

### bigcommerce/channel/connection_changed


Triggered when the channel(s) connected to the site have changed

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`channel` | `\WP_Term` | The Channel term updated
`status` | `string` | The status set on the channel

Source: [src/BigCommerce/Settings/Sections/Channels.php](BigCommerce/Settings/Sections/Channels.php), [line 304](BigCommerce/Settings/Sections/Channels.php#L304-L310)

Source: [src/BigCommerce/Settings/Sections/Channels.php](BigCommerce/Settings/Sections/Channels.php), [line 322](BigCommerce/Settings/Sections/Channels.php#L322-L328)

Source: [src/BigCommerce/Settings/Sections/Channels.php](BigCommerce/Settings/Sections/Channels.php), [line 364](BigCommerce/Settings/Sections/Channels.php#L364-L370)

### bigcommerce/settings/render/currency

Source: [src/BigCommerce/Settings/Sections/Currency.php](BigCommerce/Settings/Sections/Currency.php), [line 89](BigCommerce/Settings/Sections/Currency.php#L89-L89)

### bigcommerce/settings/render/product_reviews

Source: [src/BigCommerce/Settings/Sections/Reviews.php](BigCommerce/Settings/Sections/Reviews.php), [line 29](BigCommerce/Settings/Sections/Reviews.php#L29-L29)

### bigcommerce/settings/render/credentials


Renders API credentials description for the credentials section.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`container` | `array` | Dependency injection container.

Source: [src/BigCommerce/Settings/Sections/Api_Credentials.php](BigCommerce/Settings/Sections/Api_Credentials.php), [line 31](BigCommerce/Settings/Sections/Api_Credentials.php#L31-L36)

### bigcommerce/settings/api_credentials_updated


Fires (once per pageload) when an API credential setting updates.

**Arguments**

No arguments.

Source: [src/BigCommerce/Settings/Sections/Api_Credentials.php](BigCommerce/Settings/Sections/Api_Credentials.php), [line 213](BigCommerce/Settings/Sections/Api_Credentials.php#L213-L216)

### Webhook_Cron_Tasks::UPDATE_PRODUCT


Triggered by the cron task to update a product.

Handles the product update process for the specified product ID.
Piggyback on the update handler already hooked in for handling webhook requests.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`product_id` | `int` | The ID of the product to update.

Source: [src/BigCommerce/Post_Types/Product/Single_Product_Sync.php](BigCommerce/Post_Types/Product/Single_Product_Sync.php), [line 130](BigCommerce/Post_Types/Product/Single_Product_Sync.php#L130-L140)

### bigcommerce/channel/error/could_not_fetch_listing


Error triggered when fetching a listing fails

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`channel_id` | `int` | 
`listing_id` | `int` | 
`e` | `\BigCommerce\Api\v3\ApiException` | 

Source: [src/BigCommerce/Post_Types/Product/Channel_Sync.php](BigCommerce/Post_Types/Product/Channel_Sync.php), [line 65](BigCommerce/Post_Types/Product/Channel_Sync.php#L65-L72)

Source: [src/BigCommerce/Post_Types/Product/Channel_Sync.php](BigCommerce/Post_Types/Product/Channel_Sync.php), [line 108](BigCommerce/Post_Types/Product/Channel_Sync.php#L108-L115)

Source: [src/BigCommerce/Post_Types/Product/Channel_Sync.php](BigCommerce/Post_Types/Product/Channel_Sync.php), [line 214](BigCommerce/Post_Types/Product/Channel_Sync.php#L214-L221)

### bigcommerce/channel/error/could_not_update_listing


Error triggered when updating a listing fails

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`channel_id` | `int` | 
`listing_id` | `int` | 
`e` | `\BigCommerce\Api\v3\ApiException` | 

Source: [src/BigCommerce/Post_Types/Product/Channel_Sync.php](BigCommerce/Post_Types/Product/Channel_Sync.php), [line 91](BigCommerce/Post_Types/Product/Channel_Sync.php#L91-L98)

Source: [src/BigCommerce/Post_Types/Product/Channel_Sync.php](BigCommerce/Post_Types/Product/Channel_Sync.php), [line 240](BigCommerce/Post_Types/Product/Channel_Sync.php#L240-L247)

### bigcommerce/query/sort

Source: [src/BigCommerce/Post_Types/Product/Query.php](BigCommerce/Post_Types/Product/Query.php), [line 216](BigCommerce/Post_Types/Product/Query.php#L216-L216)

### bigcommerce/channel/promote


Triggers the promotion of a channel to the "Primary" state

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`term` | `\WP_Term` | The Channel term associated with the BigCommerce channel

Source: [src/BigCommerce/Taxonomies/Channel/Channel_Connector.php](BigCommerce/Taxonomies/Channel/Channel_Connector.php), [line 66](BigCommerce/Taxonomies/Channel/Channel_Connector.php#L66-L71)

Source: [src/BigCommerce/Taxonomies/Channel/Channel_Connector.php](BigCommerce/Taxonomies/Channel/Channel_Connector.php), [line 148](BigCommerce/Taxonomies/Channel/Channel_Connector.php#L148-L153)

### bigcommerce/channel/error/could_not_create_channel

Source: [src/BigCommerce/Taxonomies/Channel/Channel_Connector.php](BigCommerce/Taxonomies/Channel/Channel_Connector.php), [line 109](BigCommerce/Taxonomies/Channel/Channel_Connector.php#L109-L109)

### bigcommerce/update_site_home/error

Source: [src/BigCommerce/Taxonomies/Channel/Routes.php](BigCommerce/Taxonomies/Channel/Routes.php), [line 128](BigCommerce/Taxonomies/Channel/Routes.php#L128-L128)

### bigcommerce/channel/error/could_not_update_route

Source: [src/BigCommerce/Taxonomies/Channel/Routes.php](BigCommerce/Taxonomies/Channel/Routes.php), [line 348](BigCommerce/Taxonomies/Channel/Routes.php#L348-L348)

### bigcommerce/action_endpoint/{$endpoint}


Action hook that handles requests for various endpoints.

For example, the hook is triggered when the `bigcommerce/action_endpoint/<ACTION>` endpoint
for the `Buy_Now` action is called. This would process the Buy Now request and handles
adding the item to the cart.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`args` | `array` | The arguments passed to the action (e.g., product details).

Source: [src/BigCommerce/Rewrites/Action_Endpoint.php](BigCommerce/Rewrites/Action_Endpoint.php), [line 30](BigCommerce/Rewrites/Action_Endpoint.php#L30-L41)

### bigcommerce/form/action={$action}[bc-action]


Fires when a BigCommerce form action is submitted.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`submission` | `array` | The sanitized form submission data (typically from $_REQUEST)

Source: [src/BigCommerce/Container/Forms.php](BigCommerce/Container/Forms.php), [line 130](BigCommerce/Container/Forms.php#L130-L135)

### bigcommerce/import/task_manager/init


Triggered when the task manager for the import has finished initializing

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`manager` | `\BigCommerce\Import\Task_Manager` | The task manager object

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 611](BigCommerce/Container/Import.php#L611-L616)

## Filters

### bigcommerce/onboarding/success_redirect


Filters onboarding success redirect.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`success_redirect` | `string` | URL.

Source: [src/BigCommerce/Merchant/Connect_Account.php](BigCommerce/Merchant/Connect_Account.php), [line 75](BigCommerce/Merchant/Connect_Account.php#L75-L80)

Source: [src/BigCommerce/Merchant/Account_Status.php](BigCommerce/Merchant/Account_Status.php), [line 119](BigCommerce/Merchant/Account_Status.php#L119-L122)

### bigcommerce/onboarding/error_redirect


Filters onboarding error redirect.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`success_redirect` | `string` | URL.

Source: [src/BigCommerce/Merchant/Connect_Account.php](BigCommerce/Merchant/Connect_Account.php), [line 84](BigCommerce/Merchant/Connect_Account.php#L84-L89)

Source: [src/BigCommerce/Merchant/Account_Status.php](BigCommerce/Merchant/Account_Status.php), [line 73](BigCommerce/Merchant/Account_Status.php#L73-L73)

### bigcommerce/oauth_connector/installation_url


Filters oauth connector installation url.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | Url.

Source: [src/BigCommerce/Merchant/Onboarding_Api.php](BigCommerce/Merchant/Onboarding_Api.php), [line 96](BigCommerce/Merchant/Onboarding_Api.php#L96-L101)

### bigcommerce/settings/next-steps/required


Filter the array of next steps required for setting up the
BigCommerce store.

**Arguments**

No arguments.

Source: [src/BigCommerce/Merchant/Setup_Status.php](BigCommerce/Merchant/Setup_Status.php), [line 212](BigCommerce/Merchant/Setup_Status.php#L212-L221)

### bigcommerce/settings/next-steps/optional


Filter the array of optional next steps for setting up the
BigCommerce store.

**Arguments**

No arguments.

Source: [src/BigCommerce/Merchant/Setup_Status.php](BigCommerce/Merchant/Setup_Status.php), [line 256](BigCommerce/Merchant/Setup_Status.php#L256-L265)

### bigcommerce/logger/formatter

Source: [src/BigCommerce/Logging/Error_Log.php](BigCommerce/Logging/Error_Log.php), [line 71](BigCommerce/Logging/Error_Log.php#L71-L71)

### bigcommerce/logger/channel

Source: [src/BigCommerce/Logging/Error_Log.php](BigCommerce/Logging/Error_Log.php), [line 74](BigCommerce/Logging/Error_Log.php#L74-L74)

### bigcommerce/logger/handler

Source: [src/BigCommerce/Logging/Error_Log.php](BigCommerce/Logging/Error_Log.php), [line 85](BigCommerce/Logging/Error_Log.php#L85-L85)

### bigcommerce/logger/level


Filter the logging level. Defaults to 'debug'.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`` | `string\|int` | The logging level, as either a PSR-3 LogLevel string or a Monolog integer.

Source: [src/BigCommerce/Logging/Error_Log.php](BigCommerce/Logging/Error_Log.php), [line 104](BigCommerce/Logging/Error_Log.php#L104-L109)

### bigcommerce/css/customizer_styles


Filters customizer styles CSS.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`css` | `string` | The styles.

Source: [src/BigCommerce/Customizer/Styles.php](BigCommerce/Customizer/Styles.php), [line 67](BigCommerce/Customizer/Styles.php#L67-L72)

### bigcommerce/product/archive/sort_options


Filter the sorting options available in the BigCommerce catalog

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`choices` | `array` | The sorting options to use

Source: [src/BigCommerce/Customizer/Sections/Product_Archive.php](BigCommerce/Customizer/Sections/Product_Archive.php), [line 261](BigCommerce/Customizer/Sections/Product_Archive.php#L261-L266)

### bigcommerce/product/archive/filter_options


Filter the filtering options available in the BigCommerce catalog

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`choices` | `array` | The filtering options to use

Source: [src/BigCommerce/Customizer/Sections/Product_Archive.php](BigCommerce/Customizer/Sections/Product_Archive.php), [line 316](BigCommerce/Customizer/Sections/Product_Archive.php#L316-L321)

### bigcommerce/proxy/request_headers


Filter the request headers.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`` | `array` | Header KV pairs.
`route` | `string` | Route requested.
`request` | `\WP_REST_Request` | API request.

Source: [src/BigCommerce/Proxy/Proxy_Controller.php](BigCommerce/Proxy/Proxy_Controller.php), [line 280](BigCommerce/Proxy/Proxy_Controller.php#L280-L297)

### bigcommerce/proxy/response_override


Filters whether the REST request should run.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`request` | `\WP_REST_Request` | 

Source: [src/BigCommerce/Proxy/Proxy_Controller.php](BigCommerce/Proxy/Proxy_Controller.php), [line 307](BigCommerce/Proxy/Proxy_Controller.php#L307-L312)

### bigcommerce/proxy/request


Filters a proxy REST request before it is run.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`request` | `\WP_REST_Request` | Original request.

Source: [src/BigCommerce/Proxy/Proxy_Controller.php](BigCommerce/Proxy/Proxy_Controller.php), [line 324](BigCommerce/Proxy/Proxy_Controller.php#L324-L329)

### bigcommerce/proxy/result_pre


Pre-fetch results. Can be from database or from cache.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`` | `array` | Empty array.
`request` | `\WP_REST_Request` | API request.
`` | `array` | Proxy configuration.

Source: [src/BigCommerce/Proxy/Proxy_Controller.php](BigCommerce/Proxy/Proxy_Controller.php), [line 338](BigCommerce/Proxy/Proxy_Controller.php#L338-L345)

### bigcommerce/proxy/result


Filter the response results before returning it.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`result` | `array\|\WP_Error` | Result from API call.
`route` | `string` | Route requested.
`request` | `\WP_REST_Request` | API request.

Source: [src/BigCommerce/Proxy/Proxy_Controller.php](BigCommerce/Proxy/Proxy_Controller.php), [line 388](BigCommerce/Proxy/Proxy_Controller.php#L388-L395)

### bigcommerce/proxy/rest_response


Filter the WordPress REST response before it gets dispatched.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`rest_response` | `\WP_REST_Response` | Response to send back to request..
`route` | `string` | Route requested.
`request` | `\WP_REST_Request` | API request.

Source: [src/BigCommerce/Proxy/Proxy_Controller.php](BigCommerce/Proxy/Proxy_Controller.php), [line 399](BigCommerce/Proxy/Proxy_Controller.php#L399-L406)

### bigcommerce/proxy/request_url


Filters proxy request url.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`route` | `string` | Request url.
`request` | `\WP_REST_Request` | Request.

Source: [src/BigCommerce/Proxy/Proxy_Controller.php](BigCommerce/Proxy/Proxy_Controller.php), [line 676](BigCommerce/Proxy/Proxy_Controller.php#L676-L682)

### bigcommerce/currency/format


This filter is documented in src/BigCommerce/Currency/With_Currency.php.

**Arguments**

No arguments.

Source: [src/BigCommerce/Cart/Cart_Mapper.php](BigCommerce/Cart/Cart_Mapper.php), [line 262](BigCommerce/Cart/Cart_Mapper.php#L262-L265)

Source: [src/BigCommerce/Proxy/AMP_Cart_Controller.php](BigCommerce/Proxy/AMP_Cart_Controller.php), [line 75](BigCommerce/Proxy/AMP_Cart_Controller.php#L75-L79)

Source: [src/BigCommerce/Proxy/AMP_Cart_Controller.php](BigCommerce/Proxy/AMP_Cart_Controller.php), [line 141](BigCommerce/Proxy/AMP_Cart_Controller.php#L141-L145)

Source: [src/BigCommerce/Proxy/AMP_Cart_Controller.php](BigCommerce/Proxy/AMP_Cart_Controller.php), [line 204](BigCommerce/Proxy/AMP_Cart_Controller.php#L204-L204)

Source: [src/BigCommerce/Cart/Cart_Mapper.php](BigCommerce/Cart/Cart_Mapper.php), [line 363](BigCommerce/Cart/Cart_Mapper.php#L363-L366)

Source: [src/BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php), [line 183](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php#L183-L186)

Source: [src/BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php), [line 187](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php#L187-L190)

Source: [src/BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php), [line 218](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php#L218-L221)

Source: [src/BigCommerce/Currency/With_Currency.php](BigCommerce/Currency/With_Currency.php), [line 24](BigCommerce/Currency/With_Currency.php#L24-L30)

Source: [src/BigCommerce/Templates/Gift_Certificate_Balance_Response.php](BigCommerce/Templates/Gift_Certificate_Balance_Response.php), [line 37](BigCommerce/Templates/Gift_Certificate_Balance_Response.php#L37-L40)

Source: [src/BigCommerce/Rest/Shipping_Controller.php](BigCommerce/Rest/Shipping_Controller.php), [line 317](BigCommerce/Rest/Shipping_Controller.php#L317-L320)

Source: [src/BigCommerce/Rest/Coupon_Code_Controller.php](BigCommerce/Rest/Coupon_Code_Controller.php), [line 153](BigCommerce/Rest/Coupon_Code_Controller.php#L153-L156)

### bigcommerce/cart/cart_id


Filter the cart ID to use for the current request.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`cart_id` | `string` | The current cart ID.

Source: [src/BigCommerce/Cart/Cart.php](BigCommerce/Cart/Cart.php), [line 60](BigCommerce/Cart/Cart.php#L60-L65)

### bigcommerce/cart/cookie_lifetime


Filter how long the cart cookie should persist.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`lifetime` | `int` | The cookie lifespan in seconds.

Source: [src/BigCommerce/Cart/Cart.php](BigCommerce/Cart/Cart.php), [line 78](BigCommerce/Cart/Cart.php#L78-L83)

### bigcommerce/cart/permalink


Filter the URL to the cart page

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The URL to the cart page
`page_id` | `int` | The ID of the cart page

Source: [src/BigCommerce/Cart/Cart.php](BigCommerce/Cart/Cart.php), [line 268](BigCommerce/Cart/Cart.php#L268-L274)

Source: [src/BigCommerce/Amp/Amp_Cart.php](BigCommerce/Amp/Amp_Cart.php), [line 84](BigCommerce/Amp/Amp_Cart.php#L84-L90)

### bigcommerce/checkout/url


Filters checkout url.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`checkout_url` | `string` | The URL for checking out with the given cart.

Source: [src/BigCommerce/Cart/Cart.php](BigCommerce/Cart/Cart.php), [line 296](BigCommerce/Cart/Cart.php#L296-L301)

Source: [src/BigCommerce/Cart/Cart.php](BigCommerce/Cart/Cart.php), [line 325](BigCommerce/Cart/Cart.php#L325-L330)

Source: [src/BigCommerce/Cart/Checkout.php](BigCommerce/Cart/Checkout.php), [line 79](BigCommerce/Cart/Checkout.php#L79-L82)

### bigcommerce/currency/code


Filters the currency code.

This filter allows modification of the currency code being used. It returns
the current currency code based on the configured currency.

**Arguments**

No arguments.

Source: [src/BigCommerce/Cart/Cart.php](BigCommerce/Cart/Cart.php), [line 347](BigCommerce/Cart/Cart.php#L347-L355)

Source: [src/BigCommerce/Forms/Switch_Currency_Handler.php](BigCommerce/Forms/Switch_Currency_Handler.php), [line 80](BigCommerce/Forms/Switch_Currency_Handler.php#L80-L80)

Source: [src/BigCommerce/Widgets/Currency_Switcher_Widget.php](BigCommerce/Widgets/Currency_Switcher_Widget.php), [line 66](BigCommerce/Widgets/Currency_Switcher_Widget.php#L66-L66)

Source: [src/BigCommerce/Rest/Pricing_Controller.php](BigCommerce/Rest/Pricing_Controller.php), [line 88](BigCommerce/Rest/Pricing_Controller.php#L88-L88)

Source: [src/BigCommerce/Assets/Theme/JS_Config.php](BigCommerce/Assets/Theme/JS_Config.php), [line 70](BigCommerce/Assets/Theme/JS_Config.php#L70-L70)

### bigcommerce/cart/mini-cart-enabled


Filter whether the mini-cart widget should be enabled on the current page

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`enabled` | `bool` | Whether the mini-cart is enabled

Source: [src/BigCommerce/Cart/Mini_Cart.php](BigCommerce/Cart/Mini_Cart.php), [line 47](BigCommerce/Cart/Mini_Cart.php#L47-L52)

### bigcommerce/cart_mapper/map


Filter mapped cart

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`cart` | `array` | Cart data.

Source: [src/BigCommerce/Cart/Cart_Mapper.php](BigCommerce/Cart/Cart_Mapper.php), [line 109](BigCommerce/Cart/Cart_Mapper.php#L109-L114)

### bigcommerce/cart/menu/show_count


Filter whether the site should show the cart count on the menu
item for the cart page.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`show` | `bool` | Whether the cart count will be displayed

Source: [src/BigCommerce/Cart/Cart_Menu_Item.php](BigCommerce/Cart/Cart_Menu_Item.php), [line 73](BigCommerce/Cart/Cart_Menu_Item.php#L73-L79)

### bigcommerce/form/address/created_message


Filters address form created message.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`message` | `string` | Message.

Source: [src/BigCommerce/Forms/Update_Address_Handler.php](BigCommerce/Forms/Update_Address_Handler.php), [line 66](BigCommerce/Forms/Update_Address_Handler.php#L66-L71)

### bigcommerce/form/address/updated_message


Filters address form updated message.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`message` | `string` | Message.

Source: [src/BigCommerce/Forms/Update_Address_Handler.php](BigCommerce/Forms/Update_Address_Handler.php), [line 74](BigCommerce/Forms/Update_Address_Handler.php#L74-L79)

### bigcommerce/form/update_address/errors


Filters update profile address form errors.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`errors` | `\WP_Error` | WP error.
`submission` | `array` | Submitted data.

Source: [src/BigCommerce/Forms/Update_Address_Handler.php](BigCommerce/Forms/Update_Address_Handler.php), [line 138](BigCommerce/Forms/Update_Address_Handler.php#L138-L144)

### bigcommerce/form/redirect_url


Filter the redirect URL after a form submission.

Return `false` to abort the redirect.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The destination URL of the redirect.

Source: [src/BigCommerce/Forms/Form_Redirect.php](BigCommerce/Forms/Form_Redirect.php), [line 23](BigCommerce/Forms/Form_Redirect.php#L23-L29)

### bigcommerce/forms/show_messages

Source: [src/BigCommerce/Forms/Messages.php](BigCommerce/Forms/Messages.php), [line 41](BigCommerce/Forms/Messages.php#L41-L41)

### bigcommerce/forms/messages


Filter the feedback messages that will be rendered.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`messages` | `string` | The rendered messages.

Source: [src/BigCommerce/Forms/Messages.php](BigCommerce/Forms/Messages.php), [line 45](BigCommerce/Forms/Messages.php#L45-L50)

Source: [src/BigCommerce/Templates/Review_Form.php](BigCommerce/Templates/Review_Form.php), [line 101](BigCommerce/Templates/Review_Form.php#L101-L106)

### bigcommerce/forms/show_error_messages

Source: [src/BigCommerce/Forms/Messages.php](BigCommerce/Forms/Messages.php), [line 97](BigCommerce/Forms/Messages.php#L97-L97)

### bigcommerce/forms/show_success_messages

Source: [src/BigCommerce/Forms/Messages.php](BigCommerce/Forms/Messages.php), [line 139](BigCommerce/Forms/Messages.php#L139-L139)

### bigcommerce/messages/success/arguments


Filter the arguments passed to the success message template.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`args` | `array` | The arguments that will be passed.
`data` | `array` | The data that was stored with the message.

Source: [src/BigCommerce/Forms/Messages.php](BigCommerce/Forms/Messages.php), [line 150](BigCommerce/Forms/Messages.php#L150-L156)

### bigcommerce/form/delete_address/errors


Filters delete address form errors.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`errors` | `\WP_Error` | WP error.
`submission` | `array` | Submitted data.

Source: [src/BigCommerce/Forms/Delete_Address_Handler.php](BigCommerce/Forms/Delete_Address_Handler.php), [line 83](BigCommerce/Forms/Delete_Address_Handler.php#L83-L89)

### bigcommerce/user/default_role


This filter is documented in src/BigCommerce/Accounts/Login.php

**Arguments**

No arguments.

Source: [src/BigCommerce/Forms/Registration_Handler.php](BigCommerce/Forms/Registration_Handler.php), [line 152](BigCommerce/Forms/Registration_Handler.php#L152-L153)

Source: [src/BigCommerce/Accounts/Login.php](BigCommerce/Accounts/Login.php), [line 238](BigCommerce/Accounts/Login.php#L238-L243)

Source: [src/BigCommerce/Accounts/Login.php](BigCommerce/Accounts/Login.php), [line 454](BigCommerce/Accounts/Login.php#L454-L459)

Source: [src/BigCommerce/Webhooks/Customer/Customer_Creator.php](BigCommerce/Webhooks/Customer/Customer_Creator.php), [line 62](BigCommerce/Webhooks/Customer/Customer_Creator.php#L62-L67)

### bigcommerce/form/registration/success_message


The message to display when an account is created

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`message` | `string` | 

Source: [src/BigCommerce/Forms/Registration_Handler.php](BigCommerce/Forms/Registration_Handler.php), [line 170](BigCommerce/Forms/Registration_Handler.php#L170-L175)

### bigcommerce/form/registration/errors


Filters update registration form errors.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`errors` | `\WP_Error` | WP error.
`submission` | `array` | Submitted data.

Source: [src/BigCommerce/Forms/Registration_Handler.php](BigCommerce/Forms/Registration_Handler.php), [line 274](BigCommerce/Forms/Registration_Handler.php#L274-L280)

### bigcommerce/form/currency_switch/success_message


The message to display on currency switch

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`message` | `string` | 

Source: [src/BigCommerce/Forms/Switch_Currency_Handler.php](BigCommerce/Forms/Switch_Currency_Handler.php), [line 97](BigCommerce/Forms/Switch_Currency_Handler.php#L97-L102)

### bigcommerce/form/switch_currency/errors

Source: [src/BigCommerce/Forms/Switch_Currency_Handler.php](BigCommerce/Forms/Switch_Currency_Handler.php), [line 146](BigCommerce/Forms/Switch_Currency_Handler.php#L146-L146)

### bigcommerce/form/review/status

Source: [src/BigCommerce/Forms/Product_Review_Handler.php](BigCommerce/Forms/Product_Review_Handler.php), [line 74](BigCommerce/Forms/Product_Review_Handler.php#L74-L74)

### bigcommerce/form/review/created_message


Filters review form created message.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`message` | `string` | Message displayed after review submission.

Source: [src/BigCommerce/Forms/Product_Review_Handler.php](BigCommerce/Forms/Product_Review_Handler.php), [line 96](BigCommerce/Forms/Product_Review_Handler.php#L96-L101)

### bigcommerce/product/reviews/show_form

Source: [src/BigCommerce/Forms/Product_Review_Handler.php](BigCommerce/Forms/Product_Review_Handler.php), [line 123](BigCommerce/Forms/Product_Review_Handler.php#L123-L123)

Source: [src/BigCommerce/Templates/Product_Reviews.php](BigCommerce/Templates/Product_Reviews.php), [line 73](BigCommerce/Templates/Product_Reviews.php#L73-L73)

### bigcommerce/form/review/errors


Filters update review form errors.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`errors` | `\WP_Error` | WP error.
`submission` | `array` | Submitted data.

Source: [src/BigCommerce/Forms/Product_Review_Handler.php](BigCommerce/Forms/Product_Review_Handler.php), [line 155](BigCommerce/Forms/Product_Review_Handler.php#L155-L161)

### bigcommerce/form/profile/success_message


Filters profile form success message.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`message` | `string` | Profile form success message.

Source: [src/BigCommerce/Forms/Update_Profile_Handler.php](BigCommerce/Forms/Update_Profile_Handler.php), [line 93](BigCommerce/Forms/Update_Profile_Handler.php#L93-L98)

### bigcommerce/form/update_profile/errors


Filters update profile form errors.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`errors` | `\WP_Error` | WP error.
`submission` | `array` | Submitted data.

Source: [src/BigCommerce/Forms/Update_Profile_Handler.php](BigCommerce/Forms/Update_Profile_Handler.php), [line 157](BigCommerce/Forms/Update_Profile_Handler.php#L157-L163)

### bigcommerce/form/gift_certificate/success_message


The message to display when a gift certificate is added to the cart

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`message` | `string` | 

Source: [src/BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php), [line 110](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php#L110-L115)

### bigcommerce/form/gift_certificate/errors


Filters update gift certificates form errors.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`errors` | `\WP_Error` | WP error.
`submission` | `array` | Submitted data.

Source: [src/BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php), [line 199](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php#L199-L205)

### bigcommerce/gift_certificates/theme


Filters gift certificates theme.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`theme` | `string` | Theme.

Source: [src/BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php), [line 223](BigCommerce/Forms/Purchase_Gift_Certificate_Handler.php#L223-L228)

### bigcommerce/pages/matching_page_candidates


Filters pages matching page candidates.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`post_ids` | `array` | Post ids.
`name` | `string` | Name.

Source: [src/BigCommerce/Pages/Shipping_Returns_Page.php](BigCommerce/Pages/Shipping_Returns_Page.php), [line 83](BigCommerce/Pages/Shipping_Returns_Page.php#L83-L89)

Source: [src/BigCommerce/Pages/Required_Page.php](BigCommerce/Pages/Required_Page.php), [line 208](BigCommerce/Pages/Required_Page.php#L208-L211)

Source: [src/BigCommerce/Pages/Checkout_Complete_Page.php](BigCommerce/Pages/Checkout_Complete_Page.php), [line 70](BigCommerce/Pages/Checkout_Complete_Page.php#L70-L73)

### bigcommerce/pages/insert_post_args


Filters pages insert post arguments.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`args` | `array` | Arguments.
`name` | `string` | Name.

Source: [src/BigCommerce/Pages/Required_Page.php](BigCommerce/Pages/Required_Page.php), [line 223](BigCommerce/Pages/Required_Page.php#L223-L229)

### wp_edit_nav_menu_walker


This filter is documented in wp-admin/includes/nav-menu.php

**Arguments**

No arguments.

Source: [src/BigCommerce/Nav_Menu/Nav_Items_Meta_Box.php](BigCommerce/Nav_Menu/Nav_Items_Meta_Box.php), [line 204](BigCommerce/Nav_Menu/Nav_Items_Meta_Box.php#L204-L205)

### bigcommerce/gql/query_file_path

Source: [src/BigCommerce/GraphQL/GraphQL_Processor.php](BigCommerce/GraphQL/GraphQL_Processor.php), [line 280](BigCommerce/GraphQL/GraphQL_Processor.php#L280-L280)

### bigcommerce/settings/currency/auto-format


Filter whether to apply auto-formatting to currencies.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`auto_format` | `bool` | Whether to enable auto-formatting.

Source: [src/BigCommerce/Currency/Formatter_Factory.php](BigCommerce/Currency/Formatter_Factory.php), [line 49](BigCommerce/Currency/Formatter_Factory.php#L49-L54)

### bigcommerce/currency/cookie_lifetime


Filters the lifetime of the currency code cookie.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`lifetime` | `int` | The cookie lifespan in seconds.

Source: [src/BigCommerce/Currency/Currency.php](BigCommerce/Currency/Currency.php), [line 93](BigCommerce/Currency/Currency.php#L93-L98)

### bigcommerce/product/reviews/show_reviews

Source: [src/BigCommerce/Templates/Product_Single.php](BigCommerce/Templates/Product_Single.php), [line 157](BigCommerce/Templates/Product_Single.php#L157-L157)

### bigcommerce/template/wishlist/user/image_size

Source: [src/BigCommerce/Templates/Wishlist_Product.php](BigCommerce/Templates/Wishlist_Product.php), [line 46](BigCommerce/Templates/Wishlist_Product.php#L46-L46)

### bigcommerce/rest/proxy_base


Filters the REST base use for proxy API requests.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`` | `string` | Default 'bc/v3'.

Source: [src/BigCommerce/Container/Proxy.php](BigCommerce/Container/Proxy.php), [line 76](BigCommerce/Container/Proxy.php#L76-L81)

Source: [src/BigCommerce/Templates/Amp_Cart_Summary.php](BigCommerce/Templates/Amp_Cart_Summary.php), [line 34](BigCommerce/Templates/Amp_Cart_Summary.php#L34-L34)

Source: [src/BigCommerce/Templates/Amp_Cart_items.php](BigCommerce/Templates/Amp_Cart_items.php), [line 37](BigCommerce/Templates/Amp_Cart_items.php#L37-L37)

### bigcommerce/product/inventory/should_display


Filter whether to display inventory for a product

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`show` | `bool` | Whether to show the inventory level
`product` | `\BigCommerce\Post_Types\Product\Product` | The product being displayed

Source: [src/BigCommerce/Templates/Inventory_Level.php](BigCommerce/Templates/Inventory_Level.php), [line 76](BigCommerce/Templates/Inventory_Level.php#L76-L82)

### bigcommerce/address/default_state


This filter is documented in src/BigCommerce/Templates/Address_Form.php

**Arguments**

No arguments.

Source: [src/BigCommerce/Settings/Sections/New_Account_Section.php](BigCommerce/Settings/Sections/New_Account_Section.php), [line 123](BigCommerce/Settings/Sections/New_Account_Section.php#L123-L126)

Source: [src/BigCommerce/Templates/Address_Form.php](BigCommerce/Templates/Address_Form.php), [line 43](BigCommerce/Templates/Address_Form.php#L43-L43)

Source: [src/BigCommerce/Templates/Registration_Form.php](BigCommerce/Templates/Registration_Form.php), [line 38](BigCommerce/Templates/Registration_Form.php#L38-L38)

### bigcommerce/address/default_country


This filter is documented in src/BigCommerce/Templates/Address_Form.php

**Arguments**

No arguments.

Source: [src/BigCommerce/Settings/Sections/New_Account_Section.php](BigCommerce/Settings/Sections/New_Account_Section.php), [line 127](BigCommerce/Settings/Sections/New_Account_Section.php#L127-L130)

Source: [src/BigCommerce/Templates/Address_Form.php](BigCommerce/Templates/Address_Form.php), [line 50](BigCommerce/Templates/Address_Form.php#L50-L50)

Source: [src/BigCommerce/Templates/Registration_Form.php](BigCommerce/Templates/Registration_Form.php), [line 42](BigCommerce/Templates/Registration_Form.php#L42-L42)

Source: [src/BigCommerce/Settings/Sections/New_Account_Section.php](BigCommerce/Settings/Sections/New_Account_Section.php), [line 155](BigCommerce/Settings/Sections/New_Account_Section.php#L155-L158)

### bigcommerce/countries/data


Filters countries data.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`countries` | `array` | Countries.

Source: [src/BigCommerce/Templates/Address_Form.php](BigCommerce/Templates/Address_Form.php), [line 74](BigCommerce/Templates/Address_Form.php#L74-L79)

Source: [src/BigCommerce/Templates/Shipping_Methods.php](BigCommerce/Templates/Shipping_Methods.php), [line 33](BigCommerce/Templates/Shipping_Methods.php#L33-L33)

Source: [src/BigCommerce/Templates/Registration_Form.php](BigCommerce/Templates/Registration_Form.php), [line 49](BigCommerce/Templates/Registration_Form.php#L49-L52)

Source: [src/BigCommerce/Settings/Sections/New_Account_Section.php](BigCommerce/Settings/Sections/New_Account_Section.php), [line 183](BigCommerce/Settings/Sections/New_Account_Section.php#L183-L186)

### bigcommerce/template/gallery/image_size


Filter the image size used for product gallery images

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`size` | `string` | The image size to use

Source: [src/BigCommerce/Templates/Product_Gallery.php](BigCommerce/Templates/Product_Gallery.php), [line 54](BigCommerce/Templates/Product_Gallery.php#L54-L59)

Source: [src/BigCommerce/Templates/Product_Options.php](BigCommerce/Templates/Product_Options.php), [line 247](BigCommerce/Templates/Product_Options.php#L247-L250)

Source: [src/BigCommerce/Shortcodes/Product_Components.php](BigCommerce/Shortcodes/Product_Components.php), [line 134](BigCommerce/Shortcodes/Product_Components.php#L134-L139)

### bigcommerce/template/gallery/thumbnail_size


Filter the image size used for product gallery image thumbnails

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`size` | `string` | The image size to use

Source: [src/BigCommerce/Templates/Product_Gallery.php](BigCommerce/Templates/Product_Gallery.php), [line 77](BigCommerce/Templates/Product_Gallery.php#L77-L82)

### bigcommerce/template/gallery/zoom_size


Filter the image size used for product gallery image thumbnails

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`size` | `string` | The image size to use

Source: [src/BigCommerce/Templates/Product_Gallery.php](BigCommerce/Templates/Product_Gallery.php), [line 86](BigCommerce/Templates/Product_Gallery.php#L86-L91)

Source: [src/BigCommerce/Templates/Product_Options.php](BigCommerce/Templates/Product_Options.php), [line 254](BigCommerce/Templates/Product_Options.php#L254-L257)

### bigcommerce/wishlist/detail/actions


Filter the action links that are displayed on a wishlist
detail page

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`actions` | `string[]` | The rendered action links
`wishlist` | `\BigCommerce\Accounts\Wishlists\Wishlist` | The wishlist being rendered

Source: [src/BigCommerce/Templates/Wishlist_Detail_Header.php](BigCommerce/Templates/Wishlist_Detail_Header.php), [line 74](BigCommerce/Templates/Wishlist_Detail_Header.php#L74-L81)

### bigcommerce/template/image/fallback


Filter the fallback image for products without a featured image

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`image` | `string` | The fallback image HTML

Source: [src/BigCommerce/Templates/Fallback_Image.php](BigCommerce/Templates/Fallback_Image.php), [line 47](BigCommerce/Templates/Fallback_Image.php#L47-L52)

### bigcommerce/wishlist/list/actions


Filter the action links that are displayed on a wishlist
detail page

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`actions` | `string[]` | The rendered action links
`wishlist` | `\BigCommerce\Accounts\Wishlists\Wishlist` | The wishlist being rendered

Source: [src/BigCommerce/Templates/Wishlist_List_Row.php](BigCommerce/Templates/Wishlist_List_Row.php), [line 72](BigCommerce/Templates/Wishlist_List_Row.php#L72-L79)

### bigcommerce/template/directory/theme


This filter is documented in src/BigCommerce/Templates/Controller.php

**Arguments**

No arguments.

Source: [src/BigCommerce/Templates/Template_Override.php](BigCommerce/Templates/Template_Override.php), [line 215](BigCommerce/Templates/Template_Override.php#L215-L218)

Source: [src/BigCommerce/Templates/Template_Override.php](BigCommerce/Templates/Template_Override.php), [line 164](BigCommerce/Templates/Template_Override.php#L164-L164)

Source: [src/BigCommerce/Templates/Controller.php](BigCommerce/Templates/Controller.php), [line 138](BigCommerce/Templates/Controller.php#L138-L143)

Source: [src/BigCommerce/Settings/Sections/Troubleshooting_Diagnostics.php](BigCommerce/Settings/Sections/Troubleshooting_Diagnostics.php), [line 565](BigCommerce/Settings/Sections/Troubleshooting_Diagnostics.php#L565-L570)

Source: [src/BigCommerce/Settings/Sections/Troubleshooting_Diagnostics.php](BigCommerce/Settings/Sections/Troubleshooting_Diagnostics.php), [line 658](BigCommerce/Settings/Sections/Troubleshooting_Diagnostics.php#L658-L661)

Source: [src/BigCommerce/Amp/Amp_Template_Override.php](BigCommerce/Amp/Amp_Template_Override.php), [line 53](BigCommerce/Amp/Amp_Template_Override.php#L53-L59)

### bigcommerce/template/directory/plugin


This filter is documented in src/BigCommerce/Templates/Controller.php

**Arguments**

No arguments.

Source: [src/BigCommerce/Templates/Template_Override.php](BigCommerce/Templates/Template_Override.php), [line 223](BigCommerce/Templates/Template_Override.php#L223-L226)

Source: [src/BigCommerce/Templates/Controller.php](BigCommerce/Templates/Controller.php), [line 144](BigCommerce/Templates/Controller.php#L144-L149)

Source: [src/BigCommerce/Amp/Amp_Template_Override.php](BigCommerce/Amp/Amp_Template_Override.php), [line 61](BigCommerce/Amp/Amp_Template_Override.php#L61-L67)

### bigcommerce/template/path


Filter the path to a template

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`path` | `string` | The absolute path to the template
`relative_path` | `string` | The relative path of the requested template

Source: [src/BigCommerce/Templates/Controller.php](BigCommerce/Templates/Controller.php), [line 161](BigCommerce/Templates/Controller.php#L161-L167)

Source: [src/BigCommerce/Templates/Template_Override.php](BigCommerce/Templates/Template_Override.php), [line 231](BigCommerce/Templates/Template_Override.php#L231-L231)

### bigcommerce/template/product_archive/thumbnail_size

Source: [src/BigCommerce/Templates/Product_Archive.php](BigCommerce/Templates/Product_Archive.php), [line 37](BigCommerce/Templates/Product_Archive.php#L37-L37)

### bigcommerce/template/product_list/none_option_label

Source: [src/BigCommerce/Templates/Option_Types/Option_Product_List.php](BigCommerce/Templates/Option_Types/Option_Product_List.php), [line 57](BigCommerce/Templates/Option_Types/Option_Product_List.php#L57-L57)

### bigcommerce/cart/continue_shopping_url


Filter the destination of the Continue Shopping link in an empty cart

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | 

Source: [src/BigCommerce/Templates/Cart_Empty.php](BigCommerce/Templates/Cart_Empty.php), [line 45](BigCommerce/Templates/Cart_Empty.php#L45-L50)

### bigcommerce/cart/continue_shopping_text


Filter the wording of the Continue Shopping link in an empty cart

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`link_text` | `string` | 

Source: [src/BigCommerce/Templates/Cart_Empty.php](BigCommerce/Templates/Cart_Empty.php), [line 56](BigCommerce/Templates/Cart_Empty.php#L56-L61)

### bigcommerce/template/order_history/image_size

Source: [src/BigCommerce/Templates/Order_Summary.php](BigCommerce/Templates/Order_Summary.php), [line 52](BigCommerce/Templates/Order_Summary.php#L52-L52)

Source: [src/BigCommerce/Templates/Order_Product.php](BigCommerce/Templates/Order_Product.php), [line 41](BigCommerce/Templates/Order_Product.php#L41-L41)

### bigcommerce/template/order_history/date_format

Source: [src/BigCommerce/Templates/Order_Summary.php](BigCommerce/Templates/Order_Summary.php), [line 58](BigCommerce/Templates/Order_Summary.php#L58-L58)

### bigcommerce/order/include_tax_in_subtotal


Filters order included tax subtotal.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`bool` | `bool` | True or false, default false.
`order` | `array` | Order.

Source: [src/BigCommerce/Templates/Order_Summary.php](BigCommerce/Templates/Order_Summary.php), [line 73](BigCommerce/Templates/Order_Summary.php#L73-L79)

### bigcommerce/order/payment_method_label


Filter the label displayed for a payment method

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`label` | `string` | The label to display
`method` | `string` | The payment method name

Source: [src/BigCommerce/Templates/Order_Summary.php](BigCommerce/Templates/Order_Summary.php), [line 239](BigCommerce/Templates/Order_Summary.php#L239-L245)

### bigcommerce/order/support_email


Filter the support email address displayed on order detail pages.

If empty, no email will display.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`email_address` | `string` | The email address to display, defaults to the value set on the BigCommerce setting screen

Source: [src/BigCommerce/Templates/Order_Summary.php](BigCommerce/Templates/Order_Summary.php), [line 249](BigCommerce/Templates/Order_Summary.php#L249-L255)

### bigcommerce/query/default_sort


This filter is documents in src/BigCommerce/Post_Types/Product/Query.php

**Arguments**

No arguments.

Source: [src/BigCommerce/Templates/Refinery.php](BigCommerce/Templates/Refinery.php), [line 108](BigCommerce/Templates/Refinery.php#L108-L111)

Source: [src/BigCommerce/Post_Types/Product/Query.php](BigCommerce/Post_Types/Product/Query.php), [line 76](BigCommerce/Post_Types/Product/Query.php#L76-L81)

### bigcommerce/template/controller_factory


Filter the factory class that instantiates template controllers

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`factory` | `\BigCommerce\Templates\Controller_Factory` | The instance of the factory class
`classname` | `string` | The name of the requested class

Source: [src/BigCommerce/Templates/Controller.php](BigCommerce/Templates/Controller.php), [line 39](BigCommerce/Templates/Controller.php#L39-L45)

### bigcommerce/template/options


Filter the options passed in to a template controller

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`options` | `array` | The options for the template
`template` | `string` | The template path

Source: [src/BigCommerce/Templates/Controller.php](BigCommerce/Templates/Controller.php), [line 61](BigCommerce/Templates/Controller.php#L61-L67)

### bigcommerce/template={$this->template}/options


Filter the options passed in to a template controller

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`options` | `array` | The options for the template
`template` | `string` | The template path

Source: [src/BigCommerce/Templates/Controller.php](BigCommerce/Templates/Controller.php), [line 68](BigCommerce/Templates/Controller.php#L68-L74)

### bigcommerce/template/data


Filter the data passed in to a template

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | The data for the template
`template` | `string` | The template path
`options` | `array` | The options from the template controller

Source: [src/BigCommerce/Templates/Controller.php](BigCommerce/Templates/Controller.php), [line 94](BigCommerce/Templates/Controller.php#L94-L101)

### bigcommerce/template={$this->template}/data


Filter the data passed in to a template

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | The data for the template
`template` | `string` | The template path
`options` | `array` | The options from the template controller

Source: [src/BigCommerce/Templates/Controller.php](BigCommerce/Templates/Controller.php), [line 102](BigCommerce/Templates/Controller.php#L102-L109)

### bigcommerce/template={$this->template}/output


Filter the rendered output of the template

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`output` | `string` | The rendered template
`template` | `string` | The template path
`data` | `array` | The data passed to the template
`options` | `array` | The options from the template controller

Source: [src/BigCommerce/Templates/Controller.php](BigCommerce/Templates/Controller.php), [line 111](BigCommerce/Templates/Controller.php#L111-L119)

### bigcommerce/template={$this->template}/path


Filter the path to a template

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`path` | `string` | The absolute path to the template
`relative_path` | `string` | The relative path of the requested template

Source: [src/BigCommerce/Templates/Controller.php](BigCommerce/Templates/Controller.php), [line 168](BigCommerce/Templates/Controller.php#L168-L174)

### bigcommerce/template/wrapper/tag

Source: [src/BigCommerce/Templates/Controller.php](BigCommerce/Templates/Controller.php), [line 195](BigCommerce/Templates/Controller.php#L195-L195)

### bigcommerce/template/wrapper/classes


Filter the HTML tag of the wrapper for a template

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`classes` | `string[]` | An array of class names
`template` | `string` | The template path

Source: [src/BigCommerce/Templates/Controller.php](BigCommerce/Templates/Controller.php), [line 200](BigCommerce/Templates/Controller.php#L200-L206)

### bigcommerce/template/wrapper/attributes


Filter the HTML tag attributes of the wrapper for a template.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`attributes` | `string[]` | An array of attribute names.
`template` | `string` | The template path.

Source: [src/BigCommerce/Templates/Controller.php](BigCommerce/Templates/Controller.php), [line 209](BigCommerce/Templates/Controller.php#L209-L215)

### bigcommerce/units/mass


Filters units mass.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`mass_unit` | `string` | Mass unit.

Source: [src/BigCommerce/Templates/Product_Specs.php](BigCommerce/Templates/Product_Specs.php), [line 40](BigCommerce/Templates/Product_Specs.php#L40-L45)

### bigcommerce/units/length


Filters units mass.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`length_unit` | `string` | Length unit.

Source: [src/BigCommerce/Templates/Product_Specs.php](BigCommerce/Templates/Product_Specs.php), [line 46](BigCommerce/Templates/Product_Specs.php#L46-L51)

### bigcommerce/product/specs


Filters product specs.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`specs` | `array` | Specs.
`product` | `\BigCommerce\Post_Types\Product\Product` | Product.

Source: [src/BigCommerce/Templates/Product_Specs.php](BigCommerce/Templates/Product_Specs.php), [line 76](BigCommerce/Templates/Product_Specs.php#L76-L82)

### bigcommerce/gift_certificates/themes


Filters gift certificates themes.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`gift_certificate_themes` | `array` | Themes.

Source: [src/BigCommerce/Templates/Gift_Certificate_Form.php](BigCommerce/Templates/Gift_Certificate_Form.php), [line 57](BigCommerce/Templates/Gift_Certificate_Form.php#L57-L87)

### bigcommerce/product/variant_price

Source: [src/BigCommerce/Templates/Product_Options.php](BigCommerce/Templates/Product_Options.php), [line 196](BigCommerce/Templates/Product_Options.php#L196-L196)

### bigcommerce/template/featured_image/size

Source: [src/BigCommerce/Templates/Product_Featured_Image.php](BigCommerce/Templates/Product_Featured_Image.php), [line 34](BigCommerce/Templates/Product_Featured_Image.php#L34-L34)

### bigcommerce/form/state/errors


Filters form state errors.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`error_data` | `array\|null` | Error data.

Source: [src/BigCommerce/Templates/Form_Controller.php](BigCommerce/Templates/Form_Controller.php), [line 18](BigCommerce/Templates/Form_Controller.php#L18-L23)

### bigcommerce_modified_product_ids


Filters modified product ids.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`modified_product_ids` | `array` | Product ids.

Source: [src/BigCommerce/Import/Processors/Listing_Fetcher.php](BigCommerce/Import/Processors/Listing_Fetcher.php), [line 65](BigCommerce/Import/Processors/Listing_Fetcher.php#L65-L70)

### bigcommerce/import/product/post_array


Filters the product post array before saving.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`postarr` | `array` | The post data array.

Source: [src/BigCommerce/Import/Importers/Products/Product_Saver.php](BigCommerce/Import/Importers/Products/Product_Saver.php), [line 120](BigCommerce/Import/Importers/Products/Product_Saver.php#L120-L125)

### bigcommerce/import/strategy/needs_refresh


Filter whether the product should be refreshed

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`response` | `bool` | Whether the product should be refreshed
`post_id` | `int` | The ID of the product post
`product` | `\BigCommerce\Api\v3\Model\Product` | The product data from the API
`listing` | `\BigCommerce\Api\v3\Model\Listing` | The channel listing data from the API
`version` | `string` | The version of the importer

Source: [src/BigCommerce/Import/Importers/Products/Product_Strategy_Factory.php](BigCommerce/Import/Importers/Products/Product_Strategy_Factory.php), [line 125](BigCommerce/Import/Importers/Products/Product_Strategy_Factory.php#L125-L134)

### bigcommerce/import/product/menu_order


Filter the menu order assigned to the product, based on the
source product's sort_order property.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`menu_order` | `int` | The menu order to assign
`product` | `\BigCommerce\Api\v3\Model\Product` | The source product

Source: [src/BigCommerce/Import/Importers/Products/Product_Builder.php](BigCommerce/Import/Importers/Products/Product_Builder.php), [line 167](BigCommerce/Import/Importers/Products/Product_Builder.php#L167-L174)

### bigcommerce/import/product/import_images

Source: [src/BigCommerce/Import/Importers/Products/Product_Builder.php](BigCommerce/Import/Importers/Products/Product_Builder.php), [line 281](BigCommerce/Import/Importers/Products/Product_Builder.php#L281-L281)

### bigcommerce/sku/normalized/segment/num_of_characters


Filters normalized SKU segment's no of chars.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`num_of_characters` | `int` | No of chars.

Source: [src/BigCommerce/Import/Importers/Products/Product_Builder.php](BigCommerce/Import/Importers/Products/Product_Builder.php), [line 470](BigCommerce/Import/Importers/Products/Product_Builder.php#L470-L475)

### bigcommerce/sku/normalized/empty


Filters normalized empty SKU.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`repeated_string` | `string` | empty sku.

Source: [src/BigCommerce/Import/Importers/Products/Product_Builder.php](BigCommerce/Import/Importers/Products/Product_Builder.php), [line 477](BigCommerce/Import/Importers/Products/Product_Builder.php#L477-L482)

### bigcommerce/sku/normalized


Filters SKU normalized.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`normalized_sku_segments` | `array` | SKU segments.
`sku` | `string` | SKU.

Source: [src/BigCommerce/Import/Importers/Products/Product_Builder.php](BigCommerce/Import/Importers/Products/Product_Builder.php), [line 485](BigCommerce/Import/Importers/Products/Product_Builder.php#L485-L491)

### bigcommerce/import/strategy/term/needs_refresh


Filter whether the term should be refreshed

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`response` | `bool` | Whether the term should be refreshed
`term_id` | `int` | The ID of the term
`bc_term` | `array` | The term data from the API
`version` | `string` | The version of the importer

Source: [src/BigCommerce/Import/Importers/Terms/Term_Strategy_Factory.php](BigCommerce/Import/Importers/Terms/Term_Strategy_Factory.php), [line 87](BigCommerce/Import/Importers/Terms/Term_Strategy_Factory.php#L87-L95)

### bigcommerce/import/term/data


Filter category data before importing.

This filter modifies the category data based on the BigCommerce category ID.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | The original category data.
`bc_category_id` | `int` | The BigCommerce category ID.
`data` | `array` | The filtered category data after applying the filter.

Source: [src/BigCommerce/Import/Importers/Terms/Term_Saver.php](BigCommerce/Import/Importers/Terms/Term_Saver.php), [line 230](BigCommerce/Import/Importers/Terms/Term_Saver.php#L230-L239)

### bigcommerce/customer/group_info_cache_expiration


Filter the duration of the group info cache.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`expiration` | `int` | Time until expiration, in seconds.
`group_id` | `int` | The ID of the group being cached.

Source: [src/BigCommerce/Accounts/Customer_Group_Proxy.php](BigCommerce/Accounts/Customer_Group_Proxy.php), [line 72](BigCommerce/Accounts/Customer_Group_Proxy.php#L72-L78)

### bigcommerce/customer/group_info


Filters customer group info.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`default_group` | `array` | The default group data.
`group_id` | `int` | The group ID.

Source: [src/BigCommerce/Accounts/Customer_Group.php](BigCommerce/Accounts/Customer_Group.php), [line 41](BigCommerce/Accounts/Customer_Group.php#L41-L47)

### bigcommerce/customer/create/args


Filters customer create arguments.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`new_customer_data` | `array` | Customer data.

Source: [src/BigCommerce/Accounts/Login.php](BigCommerce/Accounts/Login.php), [line 103](BigCommerce/Accounts/Login.php#L103-L108)

Source: [src/BigCommerce/Accounts/Register.php](BigCommerce/Accounts/Register.php), [line 147](BigCommerce/Accounts/Register.php#L147-L152)

### bigcommerce/account/profile/permalink


Filter the URL to the account profile page

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The account profile page URL

Source: [src/BigCommerce/Accounts/Login.php](BigCommerce/Accounts/Login.php), [line 355](BigCommerce/Accounts/Login.php#L355-L360)

### bigcommerce/accounts/login/delete_missing_user

Source: [src/BigCommerce/Accounts/Login.php](BigCommerce/Accounts/Login.php), [line 540](BigCommerce/Accounts/Login.php#L540-L540)

### bigcommerce/account/do_subnav

Source: [src/BigCommerce/Accounts/Sub_Nav.php](BigCommerce/Accounts/Sub_Nav.php), [line 45](BigCommerce/Accounts/Sub_Nav.php#L45-L45)

### bigcommerce/account/subnav/links


Filter the links that show in the account subnav.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`links` | `array[]` | Each link will have the properties:<br>`url` - The URL of the link.<br>`label` - The label of the link.<br>`current` - Whether the link is to the current page.

Source: [src/BigCommerce/Accounts/Sub_Nav.php](BigCommerce/Accounts/Sub_Nav.php), [line 94](BigCommerce/Accounts/Sub_Nav.php#L94-L102)

### bigcommerce/wishlist/items


Filter the product IDs in the wishlist

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`product_ids` | `int[]` | The list of product IDs.
`wishlist` | `\BigCommerce\Accounts\Wishlists\Wishlist` | The wishlist object.

Source: [src/BigCommerce/Accounts/Wishlists/Wishlist.php](BigCommerce/Accounts/Wishlists/Wishlist.php), [line 100](BigCommerce/Accounts/Wishlists/Wishlist.php#L100-L106)

### bigcommerce/wishlist/public-url


Filter the URL for a public wishlist

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The wishlist URL.
`wishlist` | `\BigCommerce\Accounts\Wishlists\Wishlist` | The wishlist object.

Source: [src/BigCommerce/Accounts/Wishlists/Wishlist.php](BigCommerce/Accounts/Wishlists/Wishlist.php), [line 144](BigCommerce/Accounts/Wishlists/Wishlist.php#L144-L150)

### bigcommerce/wishlist/user-url


Filter the URL for a user to manage a wishlist.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The wishlist URL.
`wishlist` | `\BigCommerce\Accounts\Wishlists\Wishlist` | The wishlist object.

Source: [src/BigCommerce/Accounts/Wishlists/Wishlist.php](BigCommerce/Accounts/Wishlists/Wishlist.php), [line 167](BigCommerce/Accounts/Wishlists/Wishlist.php#L167-L173)

### bigcommerce/wishlist/edit-url


Filter the URL for posting an update to a wishlist's settings.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The form handler URL.
`wishlist` | `\BigCommerce\Accounts\Wishlists\Wishlist` | The wishlist object.

Source: [src/BigCommerce/Accounts/Wishlists/Wishlist.php](BigCommerce/Accounts/Wishlists/Wishlist.php), [line 184](BigCommerce/Accounts/Wishlists/Wishlist.php#L184-L190)

### bigcommerce/wishlist/delete-url


Filter the URL for deleting a wishlist.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The form handler URL.
`wishlist` | `\BigCommerce\Accounts\Wishlists\Wishlist` | The wishlist object.

Source: [src/BigCommerce/Accounts/Wishlists/Wishlist.php](BigCommerce/Accounts/Wishlists/Wishlist.php), [line 201](BigCommerce/Accounts/Wishlists/Wishlist.php#L201-L207)

### bigcommerce/wishlist/add-item-url


Filter the URL for adding an item to a wishlist.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The form handler URL.
`wishlist` | `\BigCommerce\Accounts\Wishlists\Wishlist` | The wishlist object.
`product_id` | `int` | The ID of the product to add.

Source: [src/BigCommerce/Accounts/Wishlists/Wishlist.php](BigCommerce/Accounts/Wishlists/Wishlist.php), [line 222](BigCommerce/Accounts/Wishlists/Wishlist.php#L222-L229)

### bigcommerce/wishlist/remove-item-url


Filter the URL for removing an item from a wishlist.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The form handler URL.
`wishlist` | `\BigCommerce\Accounts\Wishlists\Wishlist` | The wishlist object.
`product_id` | `int` | The ID of the product to remove.

Source: [src/BigCommerce/Accounts/Wishlists/Wishlist.php](BigCommerce/Accounts/Wishlists/Wishlist.php), [line 244](BigCommerce/Accounts/Wishlists/Wishlist.php#L244-L251)

### bigcommerce/wishlist/create-url


Filter the URL for creating a wishlist.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The form handler URL.

Source: [src/BigCommerce/Accounts/Wishlists/Wishlist.php](BigCommerce/Accounts/Wishlists/Wishlist.php), [line 262](BigCommerce/Accounts/Wishlists/Wishlist.php#L262-L267)

### bigcommerce/order/products


Filters order products

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`products` | `array` | Products.
`order_id` | `int` | Order ID.
`customer` | `\BigCommerce\Accounts\Customer` | The Customer object.

Source: [src/BigCommerce/Accounts/Customer.php](BigCommerce/Accounts/Customer.php), [line 245](BigCommerce/Accounts/Customer.php#L245-L252)

### bigcommerce/order/shipping_addresses


Filters order shipping addresses

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`addresses` | `array` | The shipping addresses.
`order_id` | `int` | Order ID.
`customer` | `\BigCommerce\Accounts\Customer` | The Customer object.

Source: [src/BigCommerce/Accounts/Customer.php](BigCommerce/Accounts/Customer.php), [line 266](BigCommerce/Accounts/Customer.php#L266-L273)

### bigcommerce/customer/empty_profile


Filter the base fields found in a customer profile

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`fields` | `array` | 

Source: [src/BigCommerce/Accounts/Customer.php](BigCommerce/Accounts/Customer.php), [line 296](BigCommerce/Accounts/Customer.php#L296-L308)

### bigcommerce/customer/group_id


This filter is documented in src/BigCommerce/Accounts/Customer.php

**Arguments**

No arguments.

Source: [src/BigCommerce/Accounts/Customer.php](BigCommerce/Accounts/Customer.php), [line 374](BigCommerce/Accounts/Customer.php#L374-L377)

Source: [src/BigCommerce/Accounts/Customer.php](BigCommerce/Accounts/Customer.php), [line 401](BigCommerce/Accounts/Customer.php#L401-L407)

### bigcommerce/nav/logout/title


Filters the title of the Sign Out link in the navigation menu.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`title` | `string` | The menu item title.
`menu_item` | `\WP_Post` | The menu item, a \WP_Post that has passed through wp_setup_nav_menu_item().

Source: [src/BigCommerce/Accounts/Nav_Menu.php](BigCommerce/Accounts/Nav_Menu.php), [line 58](BigCommerce/Accounts/Nav_Menu.php#L58-L64)

### bigcommerce/nav/account/title


Filters the title of the My Account link in the navigation menu.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`title` | `string` | The menu item title.
`menu_item` | `\WP_Post` | The menu item, a \WP_Post that has passed through wp_setup_nav_menu_item().

Source: [src/BigCommerce/Accounts/Nav_Menu.php](BigCommerce/Accounts/Nav_Menu.php), [line 82](BigCommerce/Accounts/Nav_Menu.php#L82-L88)

### bigcommerce/plugin/providers


Filter the service providers the power the plugin

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`providers` | `\BigCommerce\Container\Provider[]` | 

Source: [src/BigCommerce/Plugin.php](BigCommerce/Plugin.php), [line 89](BigCommerce/Plugin.php#L89-L94)

### bigcommerce/plugin/credentials_set


Filters the credentials set

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`set` | `bool` | false

Source: [src/BigCommerce/Plugin.php](BigCommerce/Plugin.php), [line 126](BigCommerce/Plugin.php#L126-L131)

### widget_title


This filter is documented in wp-includes/widgets/class-wp-widget-pages.php

**Arguments**

No arguments.

Source: [src/BigCommerce/Widgets/Currency_Switcher_Widget.php](BigCommerce/Widgets/Currency_Switcher_Widget.php), [line 45](BigCommerce/Widgets/Currency_Switcher_Widget.php#L45-L46)

Source: [src/BigCommerce/Widgets/Product_Category_Widget.php](BigCommerce/Widgets/Product_Category_Widget.php), [line 41](BigCommerce/Widgets/Product_Category_Widget.php#L41-L42)

Source: [src/BigCommerce/Widgets/Mini_Cart_Widget.php](BigCommerce/Widgets/Mini_Cart_Widget.php), [line 43](BigCommerce/Widgets/Mini_Cart_Widget.php#L43-L44)

### bigcommerce/currency/enabled

Source: [src/BigCommerce/Widgets/Currency_Switcher_Widget.php](BigCommerce/Widgets/Currency_Switcher_Widget.php), [line 65](BigCommerce/Widgets/Currency_Switcher_Widget.php#L65-L65)

### bigcommerce/widget/categories/dropdown_args

Source: [src/BigCommerce/Widgets/Product_Category_Widget.php](BigCommerce/Widgets/Product_Category_Widget.php), [line 120](BigCommerce/Widgets/Product_Category_Widget.php#L120-L120)

### bigcommerce/widget/categories/list_args

Source: [src/BigCommerce/Widgets/Product_Category_Widget.php](BigCommerce/Widgets/Product_Category_Widget.php), [line 155](BigCommerce/Widgets/Product_Category_Widget.php#L155-L155)

### bigcommerce/editor/shortcode_button/label


Filter the label of the Add Products button.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`label` | `string` | The button label.

Source: [src/BigCommerce/Editor/Add_Products_Button.php](BigCommerce/Editor/Add_Products_Button.php), [line 44](BigCommerce/Editor/Add_Products_Button.php#L44-L49)

### bigcommerce/pricing/customer_group_id


Filter the customer group ID passed to the BigCommerce API.

Null to use the default guest group. 0 to use unmodified catalog pricing.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`` | `int\|null` | The customer group ID

Source: [src/BigCommerce/Rest/Pricing_Controller.php](BigCommerce/Rest/Pricing_Controller.php), [line 81](BigCommerce/Rest/Pricing_Controller.php#L81-L87)

### bigcommerce/pricing/request_args


Filters pricing request arguments.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`args` | `array` | Arguments.
`request` | `\WP_REST_Request` | Full details about the request.

Source: [src/BigCommerce/Rest/Pricing_Controller.php](BigCommerce/Rest/Pricing_Controller.php), [line 96](BigCommerce/Rest/Pricing_Controller.php#L96-L102)

### bigcommerce/rest/shortcode/prepare_item_for_response


Filters the product data for a response.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`response` | `\WP_REST_Response` | The response object.
`post` | `\WP_Post` | Post object.
`request` | `\WP_REST_Request` | Request object.

Source: [src/BigCommerce/Rest/Shortcode_Controller.php](BigCommerce/Rest/Shortcode_Controller.php), [line 150](BigCommerce/Rest/Shortcode_Controller.php#L150-L157)

### bigcommerce/rest/shortcode/selection


Filters rest shortcode selection.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`args` | `array` | Arguments.
`request` | `\WP_REST_Request` | request.

Source: [src/BigCommerce/Rest/Shortcode_Controller.php](BigCommerce/Rest/Shortcode_Controller.php), [line 199](BigCommerce/Rest/Shortcode_Controller.php#L199-L205)

### bigcommerce/rest/shortcode/query


Filters rest shortcode query.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`args` | `array` | Arguments.
`request` | `\WP_REST_Request` | request.

Source: [src/BigCommerce/Rest/Shortcode_Controller.php](BigCommerce/Rest/Shortcode_Controller.php), [line 265](BigCommerce/Rest/Shortcode_Controller.php#L265-L271)

### bigcommerce/rest/products_query


Filters rest products query.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`args` | `array` | Arguments.
`request` | `\WP_REST_Request` | request.

Source: [src/BigCommerce/Rest/Products_Controller.php](BigCommerce/Rest/Products_Controller.php), [line 289](BigCommerce/Rest/Products_Controller.php#L289-L295)

### bigcommerce/rest/products/prepare_item_for_response


Filters the product data for a response.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`response` | `\WP_REST_Response` | The response object.
`post` | `\WP_Post` | Post object.
`request` | `\WP_REST_Request` | Request object.

Source: [src/BigCommerce/Rest/Products_Controller.php](BigCommerce/Rest/Products_Controller.php), [line 524](BigCommerce/Rest/Products_Controller.php#L524-L531)

### the_content


Filters the content to render messages above the main content.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`content` | `string` | The post content.

Source: [src/BigCommerce/Rest/Products_Controller.php](BigCommerce/Rest/Products_Controller.php), [line 600](BigCommerce/Rest/Products_Controller.php#L600-L607)

### bigcommerce/rest/product/content_trim_words_length

Source: [src/BigCommerce/Rest/Products_Controller.php](BigCommerce/Rest/Products_Controller.php), [line 613](BigCommerce/Rest/Products_Controller.php#L613-L613)

### bigcommerce/rest/missing_image


Filters rest missing image data.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`missing_image_data` | `array` | Data.

Source: [src/BigCommerce/Rest/Products_Controller.php](BigCommerce/Rest/Products_Controller.php), [line 669](BigCommerce/Rest/Products_Controller.php#L669-L678)

### bigcommerce/rest/image_sizes


Filters rest image sizes.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`sizes` | `array` | Sizes.

Source: [src/BigCommerce/Rest/Products_Controller.php](BigCommerce/Rest/Products_Controller.php), [line 833](BigCommerce/Rest/Products_Controller.php#L833-L838)

### bigcommerce/webhooks/registration_args


Filter the arguments sent to the BigCommerce API to register a webhook

**Arguments**

No arguments.

Source: [src/BigCommerce/Webhooks/Webhook.php](BigCommerce/Webhooks/Webhook.php), [line 138](BigCommerce/Webhooks/Webhook.php#L138-L141)

### bigcommerce/product_description/allowed_html


Filters product description's allowed html

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`allowed_html_tags` | `array` | Allowed HTML tags.

Source: [src/BigCommerce/Util/Kses.php](BigCommerce/Util/Kses.php), [line 19](BigCommerce/Util/Kses.php#L19-L37)

### bigcommerce/settings/import_status/current

Source: [src/BigCommerce/Settings/Import_Status.php](BigCommerce/Settings/Import_Status.php), [line 226](BigCommerce/Settings/Import_Status.php#L226-L226)

### bigcommerce/settings/import_status/previous

Source: [src/BigCommerce/Settings/Import_Status.php](BigCommerce/Settings/Import_Status.php), [line 295](BigCommerce/Settings/Import_Status.php#L295-L295)

Source: [src/BigCommerce/Settings/Import_Status.php](BigCommerce/Settings/Import_Status.php), [line 319](BigCommerce/Settings/Import_Status.php#L319-L319)

### bigcommerce/settings/connect_account_url


Filters settings connect account url.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`connect_account_url` | `string` | Connect account url.

Source: [src/BigCommerce/Settings/Screens/Welcome_Screen.php](BigCommerce/Settings/Screens/Welcome_Screen.php), [line 42](BigCommerce/Settings/Screens/Welcome_Screen.php#L42-L47)

### bigcommerce/settings/create_account_url


Filters settings create account url.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`create_account_url` | `string` | Create account url.

Source: [src/BigCommerce/Settings/Screens/Welcome_Screen.php](BigCommerce/Settings/Screens/Welcome_Screen.php), [line 51](BigCommerce/Settings/Screens/Welcome_Screen.php#L51-L56)

### bigcommerce/settings/credentials_url


Filters settings credential url.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`credential_url` | `string` | Credential url.

Source: [src/BigCommerce/Settings/Screens/Welcome_Screen.php](BigCommerce/Settings/Screens/Welcome_Screen.php), [line 60](BigCommerce/Settings/Screens/Welcome_Screen.php#L60-L65)

### bigcommerce/settings/welcome/notices


Filter the array of notices and promotions displayed on the plugin
welcome screen. The expected data is an array of arrays, each
with a 'title' and 'content' key. The values of those keys
should be HTML-safe strings.

The 'title' will be output inside an h3 tag. The 'content' will
be output inside a div tag.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`notices` | `array` | 

Source: [src/BigCommerce/Settings/Screens/Welcome_Screen.php](BigCommerce/Settings/Screens/Welcome_Screen.php), [line 73](BigCommerce/Settings/Screens/Welcome_Screen.php#L73-L84)

### bigcommerce/settings/default_new_menu_name


Filter the default name to give to an automatically generated
navigation menu when the user does not provide a value.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`name` | `string` | The menu name

Source: [src/BigCommerce/Settings/Screens/Nav_Menu_Screen.php](BigCommerce/Settings/Screens/Nav_Menu_Screen.php), [line 178](BigCommerce/Settings/Screens/Nav_Menu_Screen.php#L178-L184)

### bigcommerce/settings/header/welcome_message


Filters the message that displays at the top of the settings page

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`welcome_message` | `string` | 

Source: [src/BigCommerce/Settings/Screens/Settings_Screen.php](BigCommerce/Settings/Screens/Settings_Screen.php), [line 36](BigCommerce/Settings/Screens/Settings_Screen.php#L36-L41)

### bigcommerce/api/timeout


Filter the API connection timeout

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`timeout` | `int` | The timeout in seconds

Source: [src/BigCommerce/Container/Api.php](BigCommerce/Container/Api.php), [line 181](BigCommerce/Container/Api.php#L181-L186)

Source: [src/BigCommerce/Settings/Screens/Api_Credentials_Screen.php](BigCommerce/Settings/Screens/Api_Credentials_Screen.php), [line 87](BigCommerce/Settings/Screens/Api_Credentials_Screen.php#L87-L87)

### bigcommerce/settings/settings_url


Filters settings url.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`settings_url` | `string` | Settings url.

Source: [src/BigCommerce/Settings/Screens/Onboarding_Complete_Screen.php](BigCommerce/Settings/Screens/Onboarding_Complete_Screen.php), [line 83](BigCommerce/Settings/Screens/Onboarding_Complete_Screen.php#L83-L88)

### bigcommerce/settings/resources_url


Filters resources url.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`resources_url` | `string` | Resources url.

Source: [src/BigCommerce/Settings/Screens/Onboarding_Complete_Screen.php](BigCommerce/Settings/Screens/Onboarding_Complete_Screen.php), [line 96](BigCommerce/Settings/Screens/Onboarding_Complete_Screen.php#L96-L101)

### bigcommerce/documentation/url


Filters documentation url.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`documentation_url` | `string` | Documentation url.

Source: [src/BigCommerce/Settings/Screens/Onboarding_Complete_Screen.php](BigCommerce/Settings/Screens/Onboarding_Complete_Screen.php), [line 105](BigCommerce/Settings/Screens/Onboarding_Complete_Screen.php#L105-L110)

### bigcommerce/settings/resources/url


Filters the URL for fetching the resource data displayed on the
admin Resources screen.

Return an empty string to short-circuit the request and render
the default resources.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The URL to the resources JSON data

Source: [src/BigCommerce/Settings/Screens/Resources_Screen.php](BigCommerce/Settings/Screens/Resources_Screen.php), [line 52](BigCommerce/Settings/Screens/Resources_Screen.php#L52-L61)

### bigcommerce/settings/resources/default


Filter the default resources to display on the Resources admin page.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`default` | `array` | The default data array.

Source: [src/BigCommerce/Settings/Screens/Resources_Screen.php](BigCommerce/Settings/Screens/Resources_Screen.php), [line 119](BigCommerce/Settings/Screens/Resources_Screen.php#L119-L124)

### bigcommerce/settings/onboarding/steps


Filters the list of steps in the onboarding progress bar.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`steps` | `array[]` | The steps in the process. Properties:<br>- label  string The label for the step<br>- active bool   Whether the step is currently active
`state` | `int` | The current onboarding status

Source: [src/BigCommerce/Settings/Onboarding_Progress.php](BigCommerce/Settings/Onboarding_Progress.php), [line 75](BigCommerce/Settings/Onboarding_Progress.php#L75-L83)

### bigcommerce/checkout/can_embed


Filters whether checkout can embed or not.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`permitted` | `bool` | Can embed or not.

Source: [src/BigCommerce/Settings/Sections/Cart.php](BigCommerce/Settings/Sections/Cart.php), [line 174](BigCommerce/Settings/Sections/Cart.php#L174-L179)

### bigcommerce/diagnostics


Filter the list of diagnostic data

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`diagnostics` | `array` | 

Source: [src/BigCommerce/Settings/Sections/Troubleshooting_Diagnostics.php](BigCommerce/Settings/Sections/Troubleshooting_Diagnostics.php), [line 472](BigCommerce/Settings/Sections/Troubleshooting_Diagnostics.php#L472-L477)

### bigcommerce/settings/api/disabled/field={$option}


Filter whether to disable the API settings field

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`disabled` | `bool\|string` | Empty if the field should be enabled, a string indicating why it's disabled otherwise.

Source: [src/BigCommerce/Settings/Sections/Api_Credentials.php](BigCommerce/Settings/Sections/Api_Credentials.php), [line 129](BigCommerce/Settings/Sections/Api_Credentials.php#L129-L134)

### bigcommerce/onboarding/reset


Filters the URL to reset onboarding progress.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | The default URL for resetting onboarding.

Source: [src/BigCommerce/Settings/Start_Over.php](BigCommerce/Settings/Start_Over.php), [line 82](BigCommerce/Settings/Start_Over.php#L82-L88)

### bigcommerce/channel/listing/should_update

Source: [src/BigCommerce/Post_Types/Product/Channel_Sync.php](BigCommerce/Post_Types/Product/Channel_Sync.php), [line 50](BigCommerce/Post_Types/Product/Channel_Sync.php#L50-L50)

### bigcommerce/channel/listing/state


Filter the state to set on the channel listing for the product

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`state` | `string` | The listing state to set
`post_id` | `int` | The ID of the product post in WordPress
`listing` | `\BigCommerce\Api\v3\Model\Listing` | The listing from BigCommerce that will be updated

Source: [src/BigCommerce/Post_Types/Product/Channel_Sync.php](BigCommerce/Post_Types/Product/Channel_Sync.php), [line 146](BigCommerce/Post_Types/Product/Channel_Sync.php#L146-L153)

### bigcommerce/channel/listing/title


Filter the title to set on the channel listing for the product

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`title` | `string` | The listing title to set
`post_id` | `int` | The ID of the product post in WordPress
`listing` | `\BigCommerce\Api\v3\Model\Listing` | The listing from BigCommerce that will be updated

Source: [src/BigCommerce/Post_Types/Product/Channel_Sync.php](BigCommerce/Post_Types/Product/Channel_Sync.php), [line 157](BigCommerce/Post_Types/Product/Channel_Sync.php#L157-L164)

### bigcommerce/channel/listing/description


Filter the description to set on the channel listing for the product

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`title` | `string` | The listing description to set
`post_id` | `int` | The ID of the product post in WordPress
`listing` | `\BigCommerce\Api\v3\Model\Listing` | The listing from BigCommerce that will be updated

Source: [src/BigCommerce/Post_Types/Product/Channel_Sync.php](BigCommerce/Post_Types/Product/Channel_Sync.php), [line 168](BigCommerce/Post_Types/Product/Channel_Sync.php#L168-L175)

### bigcommerce/channel/listing/should_delete

Source: [src/BigCommerce/Post_Types/Product/Channel_Sync.php](BigCommerce/Post_Types/Product/Channel_Sync.php), [line 199](BigCommerce/Post_Types/Product/Channel_Sync.php#L199-L199)

### bigcommerce/post_type/product/capabilities

Source: [src/BigCommerce/Post_Types/Product/Config.php](BigCommerce/Post_Types/Product/Config.php), [line 31](BigCommerce/Post_Types/Product/Config.php#L31-L31)

### bigcommerce/query/recent_days

Source: [src/BigCommerce/Post_Types/Product/Query_Mapper.php](BigCommerce/Post_Types/Product/Query_Mapper.php), [line 133](BigCommerce/Post_Types/Product/Query_Mapper.php#L133-L133)

### bigcommerce/shortcode/products/query_args


Filters shortcode products query arguments.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`query_args` | `array` | Query Arguments.
`args` | `array` | Arguments.

Source: [src/BigCommerce/Post_Types/Product/Query_Mapper.php](BigCommerce/Post_Types/Product/Query_Mapper.php), [line 143](BigCommerce/Post_Types/Product/Query_Mapper.php#L143-L149)

### bigcommerce/product/price_range/data


Filter the price range data for a product

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`prices` | `array` | The price range meta for the product
`product` | `\BigCommerce\Post_Types\Product\Product` | The product object

Source: [src/BigCommerce/Post_Types/Product/Product.php](BigCommerce/Post_Types/Product/Product.php), [line 237](BigCommerce/Post_Types/Product/Product.php#L237-L243)

Source: [src/BigCommerce/Post_Types/Product/Product.php](BigCommerce/Post_Types/Product/Product.php), [line 273](BigCommerce/Post_Types/Product/Product.php#L273-L276)

### bigcommerce/product/price_range/formatted


Filter the formatted price range for a product

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`range` | `string` | The formatted price range
`product` | `\BigCommerce\Post_Types\Product\Product` | The product object
`prices` | `array` | The price range meta for the product

Source: [src/BigCommerce/Post_Types/Product/Product.php](BigCommerce/Post_Types/Product/Product.php), [line 259](BigCommerce/Post_Types/Product/Product.php#L259-L266)

### bigcommerce/product/calculated_price_range/formatted


Filter the formatted calculated price range for a product

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`range` | `string` | The formatted price range
`product` | `\BigCommerce\Post_Types\Product\Product` | The product object
`prices` | `array` | The price range meta for the product

Source: [src/BigCommerce/Post_Types/Product/Product.php](BigCommerce/Post_Types/Product/Product.php), [line 286](BigCommerce/Post_Types/Product/Product.php#L286-L293)

### bigcommerce/produce/retail_price/data


Filter the retail price of the product

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`retail_price` | `float` | The retail price of the product
`product` | `\BigCommerce\Post_Types\Product\Product` | The product object

Source: [src/BigCommerce/Post_Types/Product/Product.php](BigCommerce/Post_Types/Product/Product.php), [line 302](BigCommerce/Post_Types/Product/Product.php#L302-L308)

### bigcommerce/product/retail_price/formatted


Filter the formatted retail price for a product

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`retail_price` | `string` | The formatted retail price
`product` | `\BigCommerce\Post_Types\Product\Product` | The product object

Source: [src/BigCommerce/Post_Types/Product/Product.php](BigCommerce/Post_Types/Product/Product.php), [line 310](BigCommerce/Post_Types/Product/Product.php#L310-L316)

### bigcommerce/product/gallery


Filter the images that display in a product gallery

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`gallery` | `int[]` | The IDs of images in the gallery

Source: [src/BigCommerce/Post_Types/Product/Product.php](BigCommerce/Post_Types/Product/Product.php), [line 629](BigCommerce/Post_Types/Product/Product.php#L629-L634)

### bigcommerce/button/purchase


Filters purchase button.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`button` | `string` | Button html.
`post_id` | `int` | Post id.
`label` | `string` | Label.

Source: [src/BigCommerce/Post_Types/Product/Product.php](BigCommerce/Post_Types/Product/Product.php), [line 766](BigCommerce/Post_Types/Product/Product.php#L766-L773)

Source: [src/BigCommerce/Post_Types/Product/Product.php](BigCommerce/Post_Types/Product/Product.php), [line 732](BigCommerce/Post_Types/Product/Product.php#L732-L732)

### bigcommerce/button/purchase/attributes


Filters purchase button attributes.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`attributes` | `array` | Attributes.
`product` | `\BigCommerce\Post_Types\Product\Product` | Product.

Source: [src/BigCommerce/Post_Types/Product/Product.php](BigCommerce/Post_Types/Product/Product.php), [line 740](BigCommerce/Post_Types/Product/Product.php#L740-L746)

### bigcommerce/product/related_products


This filter is documented in src/BigCommerce/Post_Types/Product/Product.php

**Arguments**

No arguments.

Source: [src/BigCommerce/Post_Types/Product/Product.php](BigCommerce/Post_Types/Product/Product.php), [line 972](BigCommerce/Post_Types/Product/Product.php#L972-L975)

Source: [src/BigCommerce/Post_Types/Product/Product.php](BigCommerce/Post_Types/Product/Product.php), [line 981](BigCommerce/Post_Types/Product/Product.php#L981-L984)

Source: [src/BigCommerce/Post_Types/Product/Product.php](BigCommerce/Post_Types/Product/Product.php), [line 991](BigCommerce/Post_Types/Product/Product.php#L991-L997)

### bigcommerce/query/search_post_ids


Filters query search post ids.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`matches` | `array` | Post ids.
`search_phrase` | `string` | Search phrase.

Source: [src/BigCommerce/Post_Types/Product/Query.php](BigCommerce/Post_Types/Product/Query.php), [line 525](BigCommerce/Post_Types/Product/Query.php#L525-L531)

### bigcommerce/admin/js_localization


Filters admin js localization data.

Allows modification of the JS localization data before it is returned.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`js_i18n_array` | `array` | Js i18n data.

Source: [src/BigCommerce/Assets/Admin/JS_Localization.php](BigCommerce/Assets/Admin/JS_Localization.php), [line 63](BigCommerce/Assets/Admin/JS_Localization.php#L63-L70)

### bigcommerce/admin/js_config


Filters admin js config object.

Allows modification of the JS configuration data before it is returned.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | Js config data.

Source: [src/BigCommerce/Assets/Admin/JS_Config.php](BigCommerce/Assets/Admin/JS_Config.php), [line 69](BigCommerce/Assets/Admin/JS_Config.php#L69-L76)

### bigcommerce/gutenberg/js_config


Filters gutenberg js config data.

Allows modification of the Gutenberg-specific JS configuration data.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`gutenberg` | `array` | Js config data.

Source: [src/BigCommerce/Assets/Admin/JS_Config.php](BigCommerce/Assets/Admin/JS_Config.php), [line 93](BigCommerce/Assets/Admin/JS_Config.php#L93-L100)

### bigcommerce/assets/stylesheet


Filters assets stylesheet file.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`css_file` | `string` | CSS file name.

Source: [src/BigCommerce/Assets/Theme/Styles.php](BigCommerce/Assets/Theme/Styles.php), [line 51](BigCommerce/Assets/Theme/Styles.php#L51-L56)

### bigcommerce/js_localization


Filter the localization strings passed to front end scripts

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`js_i18n_array` | `array` | The localization strings

Source: [src/BigCommerce/Assets/Theme/JS_Localization.php](BigCommerce/Assets/Theme/JS_Localization.php), [line 73](BigCommerce/Assets/Theme/JS_Localization.php#L73-L78)

### bigcommerce/js_config


Filters Theme Js config.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`data` | `array` | Theme Js config.

Source: [src/BigCommerce/Assets/Theme/JS_Config.php](BigCommerce/Assets/Theme/JS_Config.php), [line 74](BigCommerce/Assets/Theme/JS_Config.php#L74-L79)

### bigcommerce/channel/default_name


Filter the name given to the auto-created channel.

Defaults to the blog's domain name.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`name` | `string` | The default channel name

Source: [src/BigCommerce/Taxonomies/Channel/Channel_Connector.php](BigCommerce/Taxonomies/Channel/Channel_Connector.php), [line 55](BigCommerce/Taxonomies/Channel/Channel_Connector.php#L55-L61)

### bigcommerce/channels/enable-multi-channel


Filter whether multi-channel support is enabled.

Enabling this feature allows site owners to
connect to multiple channels and switch between
them based on arbitrary criteria.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`enabled` | `bool` | Whether multi-channel is enabled. Defaults to false.

Source: [src/BigCommerce/Taxonomies/Channel/Channel.php](BigCommerce/Taxonomies/Channel/Channel.php), [line 25](BigCommerce/Taxonomies/Channel/Channel.php#L25-L35)

### bigcommerce/channels/map-products-to-all-channels


Filter whether multi-channel sync should sync to all channels.

Enabling this feature allows site owners to
connect to sync products to all channels or
only the channel it is assigned to.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`enabled` | `bool` | 

Source: [src/BigCommerce/Taxonomies/Channel/Channel.php](BigCommerce/Taxonomies/Channel/Channel.php), [line 44](BigCommerce/Taxonomies/Channel/Channel.php#L44-L52)

### bigcommerce/channel/routes


Filter the routes that will be set for the site

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`routes` | `\BigCommerce\Api\v3\Model\Route[]` | 

Source: [src/BigCommerce/Taxonomies/Channel/Routes.php](BigCommerce/Taxonomies/Channel/Routes.php), [line 274](BigCommerce/Taxonomies/Channel/Routes.php#L274-L279)

### bigcommerce/channel/current


Filter the channel to use for the current request. This only
fires if multi-channel support is enabled.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`channel` | `\WP_Term` | The WP term associated with the BigCommerce channel

Source: [src/BigCommerce/Taxonomies/Channel/Connections.php](BigCommerce/Taxonomies/Channel/Connections.php), [line 46](BigCommerce/Taxonomies/Channel/Connections.php#L46-L54)

### bigcommerce/taxonomy/{$this->taxonomy}/capabilities


Filter the default capabilities for taxonomy terms.

The dynamic portion of the hook is the name of the taxonomy.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`caps` | `array` | The capabilities array for the taxonomy

Source: [src/BigCommerce/Taxonomies/Taxonomy_Config.php](BigCommerce/Taxonomies/Taxonomy_Config.php), [line 90](BigCommerce/Taxonomies/Taxonomy_Config.php#L90-L97)

### bigcommerce/product_category/group_filter_terms_user_cache_time


Set the cache time for the list of term ids that a group-member user has access to.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`time` | `int` | The length of time in seconds to cache the terms.

Source: [src/BigCommerce/Taxonomies/Product_Category/Group_Filtered_Terms.php](BigCommerce/Taxonomies/Product_Category/Group_Filtered_Terms.php), [line 138](BigCommerce/Taxonomies/Product_Category/Group_Filtered_Terms.php#L138-L143)

### bigcommerce/gift_certificates/do_subnav

Source: [src/BigCommerce/Gift_Certificates/Sub_Nav.php](BigCommerce/Gift_Certificates/Sub_Nav.php), [line 45](BigCommerce/Gift_Certificates/Sub_Nav.php#L45-L45)

### bigcommerce/gift_certificates/subnav/links


Filter the links that show in the account subnav.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`links` | `array[]` | Each link will have the properties:<br>`url` - The URL of the link<br>`label` - The label of the link<br>`current` - Whether the link is to the current page

Source: [src/BigCommerce/Gift_Certificates/Sub_Nav.php](BigCommerce/Gift_Certificates/Sub_Nav.php), [line 78](BigCommerce/Gift_Certificates/Sub_Nav.php#L78-L86)

### bigcommerce/reviews/cache/per_page


Filter the number of product reviews to cache

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`count` | `int` | The max number of reviews that will be cached
`product_id` | `int` | The BigCommerce ID of the product;

Source: [src/BigCommerce/Reviews/Review_Cache.php](BigCommerce/Reviews/Review_Cache.php), [line 36](BigCommerce/Reviews/Review_Cache.php#L36-L42)

### bigcommerce/analytics/segment/settings


Filter the configuration object passed to Segment

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`settings` | `array` | Settings.

Source: [src/BigCommerce/Analytics/Segment.php](BigCommerce/Analytics/Segment.php), [line 78](BigCommerce/Analytics/Segment.php#L78-L83)

### Analytics::TRACK_BY_HOOK


Modifies the tracking data options for analytics.

This allows for customization of analytics tracking behavior.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`track_data` | `array` | Tracking data options.

Source: [src/BigCommerce/Analytics/Events/Add_To_Cart.php](BigCommerce/Analytics/Events/Add_To_Cart.php), [line 57](BigCommerce/Analytics/Events/Add_To_Cart.php#L57-L66)

Source: [src/BigCommerce/Analytics/Events/Add_To_Cart.php](BigCommerce/Analytics/Events/Add_To_Cart.php), [line 98](BigCommerce/Analytics/Events/Add_To_Cart.php#L98-L98)

Source: [src/BigCommerce/Analytics/Events/View_Product.php](BigCommerce/Analytics/Events/View_Product.php), [line 57](BigCommerce/Analytics/Events/View_Product.php#L57-L57)

Source: [src/BigCommerce/Analytics/Events/View_Product.php](BigCommerce/Analytics/Events/View_Product.php), [line 98](BigCommerce/Analytics/Events/View_Product.php#L98-L98)

### bigcommerce/amp/https_help_url


Filters the URL with information about updating the current site to HTTPS.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`` | `string` | URL.

Source: [src/BigCommerce/Amp/Amp_Admin_Notices.php](BigCommerce/Amp/Amp_Admin_Notices.php), [line 98](BigCommerce/Amp/Amp_Admin_Notices.php#L98-L106)

### bigcommerce/amp/amp_ssl_notice


Filters the AMP SSL notice text.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`` | `string` | 

Source: [src/BigCommerce/Amp/Amp_Admin_Notices.php](BigCommerce/Amp/Amp_Admin_Notices.php), [line 109](BigCommerce/Amp/Amp_Admin_Notices.php#L109-L114)

### bigcommerce/amp/admin_notices

Source: [src/BigCommerce/Amp/Amp_Admin_Notices.php](BigCommerce/Amp/Amp_Admin_Notices.php), [line 143](BigCommerce/Amp/Amp_Admin_Notices.php#L143-L143)

### bigcommerce/amp/kses_allowed_html


Filters AMP kses allowed html from BC.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`allowed_tags` | `array` | Allowed tags.

Source: [src/BigCommerce/Amp/Overrides.php](BigCommerce/Amp/Overrides.php), [line 141](BigCommerce/Amp/Overrides.php#L141-L246)

### bigcommerce/api/config


Filter the API connection configuration object

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`config` | `\BigCommerce\Api\Configuration` | 

Source: [src/BigCommerce/Container/Api.php](BigCommerce/Container/Api.php), [line 144](BigCommerce/Container/Api.php#L144-L149)

### bigcommerce/webhooks


Filter the webhooks that the plugin will register with BigCommerce

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`webhooks` | `\BigCommerce\Webhooks\Webhook[]` | 

Source: [src/BigCommerce/Container/Webhooks.php](BigCommerce/Container/Webhooks.php), [line 252](BigCommerce/Container/Webhooks.php#L252-L257)

### bigcommerce/settings/credentials_notice/excluded_screens


Filters settings credentials notice for excluded screens.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`excluded_screens` | `array` | 

Source: [src/BigCommerce/Container/Settings.php](BigCommerce/Container/Settings.php), [line 632](BigCommerce/Container/Settings.php#L632-L644)

### bigcommerce/countries/data_file


Filters the path of the countries data file.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`file` | `string` | Countries data json file path

Source: [src/BigCommerce/Container/Accounts.php](BigCommerce/Container/Accounts.php), [line 358](BigCommerce/Container/Accounts.php#L358-L363)

### bigcommerce/logger/path


Filter the path to the debug logging file

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`log_path` | `string` | The full file system path to the log file

Source: [src/BigCommerce/Container/Log.php](BigCommerce/Container/Log.php), [line 63](BigCommerce/Container/Log.php#L63-L68)

### bigcommerce/logger/custom_path


Filter the path to the debug logging file

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`log_path` | `string` | The full file system path to the log file

Source: [src/BigCommerce/Container/Log.php](BigCommerce/Container/Log.php), [line 74](BigCommerce/Container/Log.php#L74-L79)

### bigcommerce/oauth_connector/url


Filters oauth connector url

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`url` | `string` | Oauth connector URL.

Source: [src/BigCommerce/Container/Merchant.php](BigCommerce/Container/Merchant.php), [line 90](BigCommerce/Container/Merchant.php#L90-L95)

### bigcommerce/proxy/use_cache


Filters whether to use the proxy cache.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`` | `bool` | Default true.

Source: [src/BigCommerce/Container/Proxy.php](BigCommerce/Container/Proxy.php), [line 143](BigCommerce/Container/Proxy.php#L143-L148)

### bigcommerce/import/timeout


Filter the timeout for an import job. If a step in the import
takes more than this amount of time, it will be considered stalled
and a new job will take it over.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`timeout` | `int` | The timeout in seconds

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 239](BigCommerce/Container/Import.php#L239-L246)

### bigcommerce/import/task_list


Filter the tasks that will be registered for the product import

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`list` | `\BigCommerce\Import\Task_Definition[]` | The list of tasks to register

Source: [src/BigCommerce/Container/Import.php](BigCommerce/Container/Import.php), [line 596](BigCommerce/Container/Import.php#L596-L601)

### bigcommerce/rest/namespace_base


Filters REST namespace base.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`namespace` | `string` | Namespace.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 213](BigCommerce/Container/Rest.php#L213-L218)

### bigcommerce/rest/version


Filters REST version.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`version` | `int` | Version.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 222](BigCommerce/Container/Rest.php#L222-L227)

### bigcommerce/rest/cart_base


Filters REST cart base.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`cart` | `string` | Cart base.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 231](BigCommerce/Container/Rest.php#L231-L236)

### bigcommerce/rest/products_base


Filters REST products base.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`products` | `string` | Products base.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 244](BigCommerce/Container/Rest.php#L244-L249)

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 270](BigCommerce/Container/Rest.php#L270-L273)

### bigcommerce/rest/storefront_base


Filters REST products base.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`products` | `string` | Products base.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 257](BigCommerce/Container/Rest.php#L257-L262)

### bigcommerce/rest/shortcode_base


Filters REST shortcode base.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`shortcode` | `string` | Shortcode base.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 281](BigCommerce/Container/Rest.php#L281-L286)

### bigcommerce/rest/orders_shortcode_base


Filters REST orders shortcode base.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`orders_shortcode` | `string` | Orders shortcode base.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 294](BigCommerce/Container/Rest.php#L294-L299)

### bigcommerce/rest/product_component_shortcode_base


Filters REST product component shortcode base.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`component_shortcode` | `string` | Component shortcode base.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 307](BigCommerce/Container/Rest.php#L307-L312)

### bigcommerce/rest/review_list_base


Filters REST review list base.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`product_reviews` | `string` | Product reviews base.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 320](BigCommerce/Container/Rest.php#L320-L325)

### bigcommerce/rest/pricing_base


Filters REST pricing base.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`pricing` | `string` | Pricing base.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 333](BigCommerce/Container/Rest.php#L333-L338)

### bigcommerce/rest/shipping_base


Filters REST shipping base.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`shipping` | `string` | Shipping base.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 346](BigCommerce/Container/Rest.php#L346-L351)

### bigcommerce/rest/coupon_code


Filters REST coupon code base.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`coupon_code` | `string` | Coupon code base.

Source: [src/BigCommerce/Container/Rest.php](BigCommerce/Container/Rest.php), [line 359](BigCommerce/Container/Rest.php#L359-L364)

### bigcommerce/amp/templates/directory


Filter the name of the AMP template directory

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`directory` | `string` | The base name of the template directory

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 108](BigCommerce/Container/Amp.php#L108-L113)

### bigcommerce/amp/templates/enable_override


Toggles whether AMP template overrides will be used to render plugin templates

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`enable` | `bool` | Whether AMP template overrides are enabled

Source: [src/BigCommerce/Container/Amp.php](BigCommerce/Container/Amp.php), [line 182](BigCommerce/Container/Amp.php#L182-L187)

### bigcommerce/api/default_headers


Filters API default headers.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`default_headers` | `array` | An array of default header(s).

Source: [src/BigCommerce/Api/Configuration.php](BigCommerce/Api/Configuration.php), [line 24](BigCommerce/Api/Configuration.php#L24-L29)

### bigcommerce/api/ttl

Source: [src/BigCommerce/Api/Caching_Client.php](BigCommerce/Api/Caching_Client.php), [line 118](BigCommerce/Api/Caching_Client.php#L118-L118)

### bigcommerce/checkout/config


Filter the config used to render the embedded checkout.

For more details, @see https://github.com/bigcommerce/checkout-sdk-js/blob/master/docs/interfaces/embeddedcheckoutoptions.md

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`checkout_config` | `array` | 

Source: [src/BigCommerce/Shortcodes/Checkout.php](BigCommerce/Shortcodes/Checkout.php), [line 66](BigCommerce/Shortcodes/Checkout.php#L66-L72)

### bigcommerce/products/reviews/per_page

Source: [src/BigCommerce/Shortcodes/Product_Reviews.php](BigCommerce/Shortcodes/Product_Reviews.php), [line 58](BigCommerce/Shortcodes/Product_Reviews.php#L58-L58)

### bigcommerce/product/reviews/rest_url


Filters product reviews REST url.

**Arguments**

Argument | Type | Description
-------- | ---- | -----------
`base_url` | `string` | URL.
`post_id` | `int` | Post id.

Source: [src/BigCommerce/Shortcodes/Product_Reviews.php](BigCommerce/Shortcodes/Product_Reviews.php), [line 91](BigCommerce/Shortcodes/Product_Reviews.php#L91-L97)


<p align="center"><a href="https://github.com/pronamic/wp-documentor"><img src="https://cdn.jsdelivr.net/gh/pronamic/wp-documentor@main/logos/pronamic-wp-documentor.svgo-min.svg" alt="Pronamic WordPress Documentor" width="32" height="32"></a><br><em>Generated by <a href="https://github.com/pronamic/wp-documentor">Pronamic WordPress Documentor</a> <code>1.2.0</code></em><p>

