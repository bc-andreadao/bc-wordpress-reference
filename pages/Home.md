
***

# Documentation



This is an automatically generated documentation for **Documentation**.


## Namespaces


### \

#### Classes

| Class | Description |
|-------|-------------|
| [`Provider`](./classes/Provider.md) | This abstract class implements the `ServiceProviderInterface` from Pimple. It provides functionality for managing<br />callback registrations and offers a mechanism to access callbacks dynamically through the `__get` magic method.|



#### Functions

| Function | Description |
|----------|-------------|
| [`is_account_page`](./functions/is_account_page().md) | Checks if the current page is the account page.|
| [`is_cart`](./functions/is_cart().md) | Checks if the current page is the cart page.|
| [`is_checkout`](./functions/is_checkout().md) | Checks if the current page is the checkout page.|
| [`is_product`](./functions/is_product().md) | Checks if the current page is a product page.|
| [`is_product_category`](./functions/is_product_category().md) | Checks if the current page is a product category page.|
| [`is_product_tag`](./functions/is_product_tag().md) | Checks if the current page is a product tag page.|
| [`is_product_taxonomy`](./functions/is_product_taxonomy().md) | Checks if the current page is a product taxonomy page.|
| [`is_shop`](./functions/is_shop().md) | Checks if the current page is the shop page.|
| [`is_woocommerce_activated`](./functions/is_woocommerce_activated().md) | |
| [`wc`](./functions/wc().md) | Retrieves the WooCommerce facade instance from the container.|
| [`wc_get_cart_url`](./functions/wc_get_cart_url().md) | Retrieves the URL of the cart page.|
| [`wc_get_checkout_url`](./functions/wc_get_checkout_url().md) | Retrieves the URL of the checkout page.|
| [`wc_get_image_size`](./functions/wc_get_image_size().md) | Retrieves the WooCommerce image size.|
| [`wc_get_page_id`](./functions/wc_get_page_id().md) | Retrieves the ID of a WooCommerce page.|
| [`wc_get_template`](./functions/wc_get_template().md) | Retrieves and renders a WooCommerce template.|
| [`wc_get_template_html`](./functions/wc_get_template_html().md) | Retrieves the HTML content for a WooCommerce template.|
| [`wc_get_template_part`](./functions/wc_get_template_part().md) | Retrieves a template part for WooCommerce.|
| [`wc_locate_template`](./functions/wc_locate_template().md) | Locates a WooCommerce template.|
| [`wc_print_notices`](./functions/wc_print_notices().md) | Prints WooCommerce notices.|
| [`woocommerce_mini_cart`](./functions/woocommerce_mini_cart().md) | Displays the mini cart for WooCommerce.|
| [`woocommerce_reset_loop`](./functions/woocommerce_reset_loop().md) | Resets the WooCommerce loop.|
| [`wp_remove_targeted_link_rel_filters`](./functions/wp_remove_targeted_link_rel_filters().md) | Removes the filters added by wp_init_targeted_link_rel_filters()|
| [`wp_unschedule_hook`](./functions/wp_unschedule_hook().md) | Unschedules all events attached to the hook.|


### \BigCommerce

#### Classes

| Class | Description |
|-------|-------------|
| [`Api_Factory`](./classes/BigCommerce/Api_Factory.md) | |
| [`Plugin`](./classes/BigCommerce/Plugin.md) | |





### \BigCommerce\Accounts

#### Classes

| Class | Description |
|-------|-------------|
| [`Channel_Settings`](./classes/BigCommerce/Accounts/Channel_Settings.md) | Manages channel settings related to global logins, syncing customer settings,<br />and scheduling resyncs for updated global login configurations.|
| [`Countries`](./classes/BigCommerce/Accounts/Countries.md) | Class Countries|
| [`Customer`](./classes/BigCommerce/Accounts/Customer.md) | Handles customer-specific data and resources such as customer addresses, profiles, orders, and related functionalities.|
| [`Customer_Group`](./classes/BigCommerce/Accounts/Customer_Group.md) | Class Customer_Group|
| [`Customer_Group_Proxy`](./classes/BigCommerce/Accounts/Customer_Group_Proxy.md) | Class Customer_Group_Proxy|
| [`Login`](./classes/BigCommerce/Accounts/Login.md) | Handles the login and lost password logic for the BigCommerce account integration with WordPress.|
| [`Nav_Menu`](./classes/BigCommerce/Accounts/Nav_Menu.md) | Class Nav_Menu|
| [`Password_Reset`](./classes/BigCommerce/Accounts/Password_Reset.md) | Class Password_Reset|
| [`Register`](./classes/BigCommerce/Accounts/Register.md) | Class Register|
| [`Sub_Nav`](./classes/BigCommerce/Accounts/Sub_Nav.md) | Class Sub_Nav|
| [`User_Profile_Settings`](./classes/BigCommerce/Accounts/User_Profile_Settings.md) | Class User_Profile_Settings|





### \BigCommerce\Accounts\Roles

#### Classes

| Class | Description |
|-------|-------------|
| [`Customer`](./classes/BigCommerce/Accounts/Roles/Customer.md) | Class Customer|


#### Interfaces

| Interface | Description |
|-----------|-------------|
| [`Role`](./classes/BigCommerce/Accounts/Roles/Role.md) | Interface Role|



### \BigCommerce\Accounts\Wishlists

#### Classes

| Class | Description |
|-------|-------------|
| [`Add_Item_View`](./classes/BigCommerce/Accounts/Wishlists/Add_Item_View.md) | Class Add_Item_View|
| [`Missing_Wishlist`](./classes/BigCommerce/Accounts/Wishlists/Missing_Wishlist.md) | Class Missing_Wishlist|
| [`Public_Wishlist`](./classes/BigCommerce/Accounts/Wishlists/Public_Wishlist.md) | This class handles the public-facing wishlist view, including customizing the query<br />to show only products in the wishlist, setting the page title, customizing the<br />`wp_title()` function, and managing the &quot;No Results&quot; message on the wishlist page.|
| [`Wishlist`](./classes/BigCommerce/Accounts/Wishlists/Wishlist.md) | Class Wishlist|
| [`Wishlist_Public_View`](./classes/BigCommerce/Accounts/Wishlists/Wishlist_Public_View.md) | Abstract class for handling wishlist public view actions, including filtering main queries,<br />setting the page title, and modifying results when no items are found.|
| [`Wishlist_Request_Parser`](./classes/BigCommerce/Accounts/Wishlists/Wishlist_Request_Parser.md) | Class Wishlist_Request_Parser|





### \BigCommerce\Accounts\Wishlists\Actions

#### Classes

| Class | Description |
|-------|-------------|
| [`Add_Item`](./classes/BigCommerce/Accounts/Wishlists/Actions/Add_Item.md) | Handles requests for adding items to a customer&#039;s wishlist.|
| [`Create_Wishlist`](./classes/BigCommerce/Accounts/Wishlists/Actions/Create_Wishlist.md) | Handles the logic for creating a new wishlist for a customer.|
| [`Delete_Wishlist`](./classes/BigCommerce/Accounts/Wishlists/Actions/Delete_Wishlist.md) | Handles the logic for deleting a wishlist.|
| [`Edit_Wishlist`](./classes/BigCommerce/Accounts/Wishlists/Actions/Edit_Wishlist.md) | Handles the logic for editing a wishlist.|
| [`Remove_Item`](./classes/BigCommerce/Accounts/Wishlists/Actions/Remove_Item.md) | Handles the logic for removing an item from a customer&#039;s wishlist.|
| [`Request_Router`](./classes/BigCommerce/Accounts/Wishlists/Actions/Request_Router.md) | Class Request_Router|
| [`Wishlist_Action`](./classes/BigCommerce/Accounts/Wishlists/Actions/Wishlist_Action.md) | Abstract class for handling wishlist-related actions.|





### \BigCommerce\Amp

#### Classes

| Class | Description |
|-------|-------------|
| [`Amp_Admin_Notices`](./classes/BigCommerce/Amp/Amp_Admin_Notices.md) | Creates an admin notice if requirements for AMP + BC or not met.|
| [`Amp_Assets`](./classes/BigCommerce/Amp/Amp_Assets.md) | Class Amp_Assets|
| [`Amp_Cart`](./classes/BigCommerce/Amp/Amp_Cart.md) | Class Amp_Cart|
| [`Amp_Cart_Menu_Item`](./classes/BigCommerce/Amp/Amp_Cart_Menu_Item.md) | Class Amp_Cart_Menu_Item|
| [`Amp_Controller_Factory`](./classes/BigCommerce/Amp/Amp_Controller_Factory.md) | Class Amp_Controller_Factory|
| [`Amp_Template_Override`](./classes/BigCommerce/Amp/Amp_Template_Override.md) | Class Amp_Template_Override|
| [`Classic`](./classes/BigCommerce/Amp/Classic.md) | Class Classic|
| [`Overrides`](./classes/BigCommerce/Amp/Overrides.md) | Class Overrides|





### \BigCommerce\Analytics

#### Classes

| Class | Description |
|-------|-------------|
| [`Facebook_Pixel`](./classes/BigCommerce/Analytics/Facebook_Pixel.md) | Class Facebook_Pixel|
| [`Google_Analytics`](./classes/BigCommerce/Analytics/Google_Analytics.md) | Class Google_Analytics|
| [`Segment`](./classes/BigCommerce/Analytics/Segment.md) | Renders the Segment analytics tracking code on the site.|





### \BigCommerce\Analytics\Events

#### Classes

| Class | Description |
|-------|-------------|
| [`Add_To_Cart`](./classes/BigCommerce/Analytics/Events/Add_To_Cart.md) | Class Add_To_Cart|
| [`View_Product`](./classes/BigCommerce/Analytics/Events/View_Product.md) | Class View_Product|





### \BigCommerce\Api

#### Classes

| Class | Description |
|-------|-------------|
| [`Api_Config_Renewal`](./classes/BigCommerce/Api/Api_Config_Renewal.md) | Class Api_Config_Renewal|
| [`Api_Scopes_Validator`](./classes/BigCommerce/Api/Api_Scopes_Validator.md) | Validates the API scopes for several resources, ensuring that the correct permissions<br />are in place during the onboarding process. This includes validating scopes for<br />customers, orders, and payment methods.|
| [`Banners_Api`](./classes/BigCommerce/Api/Banners_Api.md) | Class Banners_Api|
| [`Base_Client`](./classes/BigCommerce/Api/Base_Client.md) | Base API client class that extends the ApiClient and manages the configuration<br />of the API client. This class is designed to handle the configuration for<br />API communication and can be extended for specific API clients.|
| [`Caching_Client`](./classes/BigCommerce/Api/Caching_Client.md) | Implements a short-term caching mechanism around API requests to reduce redundant calls,<br />particularly useful for operations like cart handling. The cache is invalidated after<br />any write operation to ensure data consistency.|
| [`Configuration`](./classes/BigCommerce/Api/Configuration.md) | Extends the base Configuration class to provide additional<br />functionality, such as filtering default headers for BigCommerce API requests.|
| [`ConfigurationRequiredException`](./classes/BigCommerce/Api/ConfigurationRequiredException.md) | A specific exception type that extends `ApiException` to signal<br />that a required configuration is missing when making API requests.|
| [`Currencies_Api`](./classes/BigCommerce/Api/Currencies_Api.md) | Handles retrieval of currencies from the BigCommerce v2 API.|
| [`Customer_Api`](./classes/BigCommerce/Api/Customer_Api.md) | Provides methods for interacting with BigCommerce customers via the v2 API.|
| [`Marketing_Api`](./classes/BigCommerce/Api/Marketing_Api.md) | Provides methods for interacting with marketing-related resources in BigCommerce,<br />including gift certificates.|
| [`Null_Client`](./classes/BigCommerce/Api/Null_Client.md) | A placeholder API client that disables API calls.|
| [`Payments_Api`](./classes/BigCommerce/Api/Payments_Api.md) | Provides methods for interacting with the Payments API in BigCommerce.|
| [`Request_Headers`](./classes/BigCommerce/Api/Request_Headers.md) | Provides functionality for adding custom headers to API requests, including plugin-specific<br />information like WordPress version, plugin version, and PHP version.|
| [`Shipping_Api`](./classes/BigCommerce/Api/Shipping_Api.md) | Handles API v2 requests for shipping data, including zones and shipping methods.|
| [`Store_Api`](./classes/BigCommerce/Api/Store_Api.md) | Handle retrieving information about the store from APIv2.|
| [`Tax_Class_Api`](./classes/BigCommerce/Api/Tax_Class_Api.md) | Handle tax data requests.|
| [`Webhooks_Api`](./classes/BigCommerce/Api/Webhooks_Api.md) | Creates an adapter class for the BC v2 API webhook endpoint.|
| [`v2ApiAdapter`](./classes/BigCommerce/Api/v2ApiAdapter.md) | Provides an adapter for interacting with the BigCommerce API. This class includes methods for<br />retrieving collections and resources, as well as creating, updating, and deleting resources.|

#### Traits

| Trait | Description |
|-------|-------------|
| [`Api_Data_Sanitizer`](./classes/BigCommerce/Api/Api_Data_Sanitizer.md) | Trait Api_Data_Sanitizer|




### \BigCommerce\Assets\Admin

#### Classes

| Class | Description |
|-------|-------------|
| [`JS_Config`](./classes/BigCommerce/Assets/Admin/JS_Config.md) | Handles the configuration for JavaScript assets in the BigCommerce admin.|
| [`JS_Localization`](./classes/BigCommerce/Assets/Admin/JS_Localization.md) | Class JS_Localization|
| [`Scripts`](./classes/BigCommerce/Assets/Admin/Scripts.md) | Handles the enqueueing and registration of admin scripts and Gutenberg-specific scripts.|
| [`Styles`](./classes/BigCommerce/Assets/Admin/Styles.md) | Handles the enqueueing and registration of admin and Gutenberg-specific CSS styles.|





### \BigCommerce\Assets\Theme

#### Classes

| Class | Description |
|-------|-------------|
| [`Image_Sizes`](./classes/BigCommerce/Assets/Theme/Image_Sizes.md) | Class Image_Sizes|
| [`JS_Config`](./classes/BigCommerce/Assets/Theme/JS_Config.md) | Handles the configuration for JavaScript data, which includes store settings,<br />product messages, channel data, and other theme-specific data required for the frontend.|
| [`JS_Localization`](./classes/BigCommerce/Assets/Theme/JS_Localization.md) | Handles the localization of JavaScript strings for the theme. This class generates an array of text<br />strings used in JavaScript, which can be filtered and sanitized before being passed to the frontend.|
| [`Scripts`](./classes/BigCommerce/Assets/Theme/Scripts.md) | Manages the enqueuing of JavaScript files for the theme. It handles the inclusion of asset files,<br />conditional script loading based on page type, and localization of JavaScript data.|
| [`Styles`](./classes/BigCommerce/Assets/Theme/Styles.md) | Manages the enqueuing of CSS stylesheets for the theme. This includes handling the inclusion of<br />asset files and applying any filters to the stylesheet before it is enqueued. It also checks the<br />theme settings to conditionally load the styles based on user preferences.|





### \BigCommerce\Banners

#### Classes

| Class | Description |
|-------|-------------|
| [`Banners`](./classes/BigCommerce/Banners/Banners.md) | Handles the management and display of banners on various pages of the BigCommerce WordPress theme. It<br />provides methods to configure JavaScript settings, fetch banners from the API, and filter banners based<br />on the current page context, visibility, and date range.|





### \BigCommerce\CLI

#### Classes

| Class | Description |
|-------|-------------|
| [`Command`](./classes/BigCommerce/CLI/Command.md) | This is an abstract base class for creating custom WP-CLI commands in the BigCommerce CLI namespace.|
| [`Import_Products`](./classes/BigCommerce/CLI/Import_Products.md) | Handles the import process for products from BigCommerce.|
| [`Reset_Plugin`](./classes/BigCommerce/CLI/Reset_Plugin.md) | Resets various options in WordPress to bring the site back to the beginning of the BigCommerce account onboarding flow.|
| [`Update_Country_Cache`](./classes/BigCommerce/CLI/Update_Country_Cache.md) | Updates the country and state cache in a JSON file located at assets/data/countries.json.|





### \BigCommerce\CLI\Documentation

#### Classes

| Class | Description |
|-------|-------------|
| [`Build_Docs`](./classes/BigCommerce/CLI/Documentation/Build_Docs.md) | Register build docs command and related functionality|
| [`Data_Importer`](./classes/BigCommerce/CLI/Documentation/Data_Importer.md) | Extends WP_Parser&#039;s Importer class to modify the import behavior for class methods and hooks.|
| [`Import_Docs`](./classes/BigCommerce/CLI/Documentation/Import_Docs.md) | Class Import_Docs|





### \BigCommerce\CLI\Resources

#### Classes

| Class | Description |
|-------|-------------|
| [`Build_Resources`](./classes/BigCommerce/CLI/Resources/Build_Resources.md) | Class Build_Resources|
| [`Resource`](./classes/BigCommerce/CLI/Resources/Resource.md) | Class Resource|
| [`Resource_Group`](./classes/BigCommerce/CLI/Resources/Resource_Group.md) | Represents a group of resources, which are categorized by a label.|





### \BigCommerce\Cache

#### Classes

| Class | Description |
|-------|-------------|
| [`Cache_Handler`](./classes/BigCommerce/Cache/Cache_Handler.md) | Cache_Handler class|





### \BigCommerce\Cart

#### Classes

| Class | Description |
|-------|-------------|
| [`Add_To_Cart`](./classes/BigCommerce/Cart/Add_To_Cart.md) | Handles requests from the Add to Cart button for products|
| [`Buy_Now`](./classes/BigCommerce/Cart/Buy_Now.md) | Handles requests from the Buy Now button for products.|
| [`Cache_Control`](./classes/BigCommerce/Cart/Cache_Control.md) | Class Cache_Control|
| [`Cart`](./classes/BigCommerce/Cart/Cart.md) | Handles cart operations such as adding line items, managing cookies, and interacting with the BigCommerce API.|
| [`Cart_Mapper`](./classes/BigCommerce/Cart/Cart_Mapper.md) | Maps a cart from the API to a standard format usable by the<br />REST API and other templates.|
| [`Cart_Menu_Item`](./classes/BigCommerce/Cart/Cart_Menu_Item.md) | The Cart_Menu_Item class is responsible for modifying WordPress navigation menu items<br />to display cart-related information. It specifically adds a cart item count to the menu<br />item representing the cart page and ensures the proper display of this count based on<br />various conditions like checkout settings and the status of the mini-cart.|
| [`Cart_Recovery`](./classes/BigCommerce/Cart/Cart_Recovery.md) | The Cart_Recovery class is responsible for handling the recovery of abandoned carts.|
| [`Checkout`](./classes/BigCommerce/Cart/Checkout.md) | Handles requests during checkout from the Buy Now button for products.|
| [`Item_Counter`](./classes/BigCommerce/Cart/Item_Counter.md) | Provides functionality to count the number of items in a BigCommerce cart.|
| [`Mini_Cart`](./classes/BigCommerce/Cart/Mini_Cart.md) | Manages the configuration and display logic for the mini-cart widget in BigCommerce.|





### \BigCommerce\Checkout

#### Classes

| Class | Description |
|-------|-------------|
| [`Customer_Login`](./classes/BigCommerce/Checkout/Customer_Login.md) | Handles customer login logic during the checkout process.|
| [`Requirements_Notice`](./classes/BigCommerce/Checkout/Requirements_Notice.md) | Shows a notice if the required configuration for checkout is not complete|





### \BigCommerce\Compatibility

#### Classes

| Class | Description |
|-------|-------------|
| [`Template_Compatibility`](./classes/BigCommerce/Compatibility/Template_Compatibility.md) | Provides compatibility functionality to override WooCommerce page templates.|


#### Interfaces

| Interface | Description |
|-----------|-------------|
| [`Spam_Checker`](./classes/BigCommerce/Compatibility/Spam_Checker.md) | Defines the contract for a spam checker, which can be used to determine whether a given content is considered spam.|



### \BigCommerce\Compatibility\Akismet

#### Classes

| Class | Description |
|-------|-------------|
| [`Akismet`](./classes/BigCommerce/Compatibility/Akismet/Akismet.md) | This class implements the Spam_Checker interface and uses the Akismet API to determine if a submission is considered spam.|





### \BigCommerce\Compatibility\Matomo

#### Classes

| Class | Description |
|-------|-------------|
| [`Matomo`](./classes/BigCommerce/Compatibility/Matomo/Matomo.md) | This class integrates BigCommerce with Matomo (formerly Piwik), a web analytics platform. It provides functionality for<br />modifying the JavaScript configuration for tracking user interactions with custom variables in Matomo.|





### \BigCommerce\Compatibility\Themes

#### Classes

| Class | Description |
|-------|-------------|
| [`Null_Theme`](./classes/BigCommerce/Compatibility/Themes/Null_Theme.md) | A placeholder class for themes that do not require any compatibility layer.|
| [`Theme`](./classes/BigCommerce/Compatibility/Themes/Theme.md) | Base class for themes, providing functionality for rendering templates and checking version compatibility.|
| [`Theme_Factory`](./classes/BigCommerce/Compatibility/Themes/Theme_Factory.md) | Factory class for creating theme instances based on template name and version.|





### \BigCommerce\Compatibility\Themes\Flatsome

#### Classes

| Class | Description |
|-------|-------------|
| [`Flatsome`](./classes/BigCommerce/Compatibility/Themes/Flatsome/Flatsome.md) | This class defines the compatibility layer for the Flatsome theme in the BigCommerce ecosystem.|





### \BigCommerce\Compatibility\Themes\Flatsome\Templates

#### Classes

| Class | Description |
|-------|-------------|
| [`Account_Links`](./classes/BigCommerce/Compatibility/Themes/Flatsome/Templates/Account_Links.md) | This class is responsible for generating the account links for the user&#039;s account page in the Flatsome theme.|





### \BigCommerce\Compatibility\WooCommerce

#### Classes

| Class | Description |
|-------|-------------|
| [`Cart`](./classes/BigCommerce/Compatibility/WooCommerce/Cart.md) | This class handles the interaction between the WooCommerce cart and BigCommerce&#039;s cart API.|
| [`Facade`](./classes/BigCommerce/Compatibility/WooCommerce/Facade.md) | This class acts as a facade for the WooCommerce cart, providing a simplified interface for interacting with the BigCommerce cart.|





### \BigCommerce\Container

#### Classes

| Class | Description |
|-------|-------------|
| [`Accounts`](./classes/BigCommerce/Container/Accounts.md) | Class Accounts|
| [`Amp`](./classes/BigCommerce/Container/Amp.md) | This class integrates AMP (Accelerated Mobile Pages) functionality into the BigCommerce platform.|
| [`Analytics`](./classes/BigCommerce/Container/Analytics.md) | Handles the registration and configuration of analytics services and events for BigCommerce.|
| [`Api`](./classes/BigCommerce/Container/Api.md) | Manages the registration and configuration of the BigCommerce API client and related services.|
| [`Assets`](./classes/BigCommerce/Container/Assets.md) | Provides asset management for the BigCommerce plugin, including scripts, styles,<br />configuration, and localization for both the admin and frontend.|
| [`Banners`](./classes/BigCommerce/Container/Banners.md) | This class is responsible for managing the banners service within the dependency injection container.|
| [`Cart`](./classes/BigCommerce/Container/Cart.md) | Cart service provider for managing cart-related functionality.|
| [`Checkout`](./classes/BigCommerce/Container/Checkout.md) | Handles the registration of checkout-related services and actions.|
| [`Cli`](./classes/BigCommerce/Container/Cli.md) | Provides CLI services for the BigCommerce plugin.|
| [`Compatibility`](./classes/BigCommerce/Container/Compatibility.md) | Provides integration with various third-party services and themes, including WooCommerce, Matomo, and Akismet.|
| [`Currency`](./classes/BigCommerce/Container/Currency.md) | Currency container provider class.|
| [`Editor`](./classes/BigCommerce/Container/Editor.md) | Loads behavior relevant to the admin post editor, including rendering custom buttons,<br />templates, and Gutenberg blocks within the WordPress admin interface. It also handles<br />the integration of the Gutenberg editor with BigCommerce blocks and assets.|
| [`Forms`](./classes/BigCommerce/Container/Forms.md) | Forms class handles various form actions within BigCommerce, such as registration, address updates, product reviews, and more.|
| [`Gift_Certificates`](./classes/BigCommerce/Container/Gift_Certificates.md) | This class provides functionality for registering and handling the gift certificates sub-navigation<br />in the BigCommerce environment. It extends the Provider class and implements a registration method<br />to add a sub-navigation to the content.|
| [`GraphQL`](./classes/BigCommerce/Container/GraphQL.md) | This class provides functionality for registering GraphQL-related services, such as various<br />query objects and a GraphQL requestor processor, in the BigCommerce container. The `register`<br />method configures these services to be accessed globally through the container.|
| [`Image`](./classes/BigCommerce/Container/Image.md) | This class provides functionality for registering image-related services and hooks related to<br />image import and CDN management within the BigCommerce container. It includes hooks that<br />determine if image import is allowed and modify image HTML to load images from a CDN if applicable.|
| [`Import`](./classes/BigCommerce/Container/Import.md) | This class handles the import process for BigCommerce data. It includes functionality<br />to manage cron jobs, process various import tasks, handle batch sizes, and trigger<br />different import-related actions.|
| [`Log`](./classes/BigCommerce/Container/Log.md) | This class is responsible for setting up logging functionality in the BigCommerce container.|
| [`Merchant`](./classes/BigCommerce/Container/Merchant.md) | Handles merchant-related onboarding and account management for BigCommerce integration.|
| [`Nav_Menu`](./classes/BigCommerce/Container/Nav_Menu.md) | Provides dependencies and behaviors for navigation menus.|
| [`Pages`](./classes/BigCommerce/Container/Pages.md) | Provides page-related services and ensures required pages exist for BigCommerce integration.|
| [`Post_Meta`](./classes/BigCommerce/Container/Post_Meta.md) | This class provides methods to handle post metadata related tasks in the container. It extends the Provider class<br />and registers dependencies related to post metadata processing within the container.|
| [`Post_Types`](./classes/BigCommerce/Container/Post_Types.md) | Handles the management of custom post types, particularly for products in the WordPress admin interface.|
| [`Proxy`](./classes/BigCommerce/Container/Proxy.md) | This class registers the proxy container that adds a Wordpress proxy layer on top of the BigCommerce API.|
| [`Rest`](./classes/BigCommerce/Container/Rest.md) | Provides RESTful controllers and endpoints for BigCommerce integration.|
| [`Reviews`](./classes/BigCommerce/Container/Reviews.md) | Provides functionality for managing reviews in the BigCommerce container.|
| [`Rewrites`](./classes/BigCommerce/Container/Rewrites.md) | Handles rewrite rules and flushing mechanisms for the BigCommerce container.|
| [`Schema`](./classes/BigCommerce/Container/Schema.md) | Manages the registration of database schema-related services and roles.|
| [`Settings`](./classes/BigCommerce/Container/Settings.md) | Provides various screens and settings for BigCommerce.|
| [`Shortcodes`](./classes/BigCommerce/Container/Shortcodes.md) | Registers shortcodes for various storefront features.|
| [`Taxonomies`](./classes/BigCommerce/Container/Taxonomies.md) | This class is responsible for managing and registering taxonomies for BigCommerce integration. It defines constants for various taxonomies and handles their configuration and filtering via WordPress hooks.|
| [`Templates`](./classes/BigCommerce/Container/Templates.md) | Handles template overrides and body class modifications<br />within the BigCommerce integration. It registers various filters to modify the template paths and<br />the body class dynamically based on the context, such as product pages, archives, taxonomies, and search results.|
| [`Theme_Customizer`](./classes/BigCommerce/Container/Theme_Customizer.md) | Registers theme customizer panels, sections, and styles in WordPress.|
| [`Util`](./classes/BigCommerce/Container/Util.md) | Class Util|
| [`Webhooks`](./classes/BigCommerce/Container/Webhooks.md) | Provider for handling BigCommerce webhooks.|
| [`Widgets`](./classes/BigCommerce/Container/Widgets.md) | Registers and manages widgets for the application.|





### \BigCommerce\Currency

#### Classes

| Class | Description |
|-------|-------------|
| [`Configurable_Formatter`](./classes/BigCommerce/Currency/Configurable_Formatter.md) | Class for configuring and formatting currency values.|
| [`Currency`](./classes/BigCommerce/Currency/Currency.md) | Handles currency operations, including fetching and setting currency codes and managing channel-aware currencies.|
| [`Formatter_Factory`](./classes/BigCommerce/Currency/Formatter_Factory.md) | Factory class to create and manage currency formatters.|
| [`Intl_Formatter`](./classes/BigCommerce/Currency/Intl_Formatter.md) | Formatter class for currency values using PHP&#039;s intl extension.|
| [`USD_Formatter`](./classes/BigCommerce/Currency/USD_Formatter.md) | Formatter class for currency values specifically in USD.|

#### Traits

| Trait | Description |
|-------|-------------|
| [`With_Currency`](./classes/BigCommerce/Currency/With_Currency.md) | Provides currency formatting functionality for classes.|

#### Interfaces

| Interface | Description |
|-----------|-------------|
| [`Currency_Formatter`](./classes/BigCommerce/Currency/Currency_Formatter.md) | Interface for formatting numeric values into currency strings.|



### \BigCommerce\Customizer

#### Classes

| Class | Description |
|-------|-------------|
| [`Styles`](./classes/BigCommerce/Customizer/Styles.md) | This class handles the customization of CSS styles for BigCommerce components.|





### \BigCommerce\Customizer\Controls

#### Classes

| Class | Description |
|-------|-------------|
| [`Multiple_Checkboxes`](./classes/BigCommerce/Customizer/Controls/Multiple_Checkboxes.md) | Class Multiple_Checkboxes|





### \BigCommerce\Customizer\Panels

#### Classes

| Class | Description |
|-------|-------------|
| [`Primary`](./classes/BigCommerce/Customizer/Panels/Primary.md) | Class Primary|





### \BigCommerce\Customizer\Sections

#### Classes

| Class | Description |
|-------|-------------|
| [`Banners`](./classes/BigCommerce/Customizer/Sections/Banners.md) | Represents the Customizer section for managing banner settings in the BigCommerce store.|
| [`Buttons`](./classes/BigCommerce/Customizer/Sections/Buttons.md) | A customizer section that handles button label settings for various BigCommerce buttons in the WordPress Customizer.|
| [`Cart`](./classes/BigCommerce/Customizer/Sections/Cart.md) | Handles the customization options for the Cart section in the WordPress Customizer.|
| [`Checkout`](./classes/BigCommerce/Customizer/Sections/Checkout.md) | Handles the customization options for the Checkout section in the WordPress Customizer.|
| [`Colors`](./classes/BigCommerce/Customizer/Sections/Colors.md) | Handles the customization constants for colors and themes in the BigCommerce plugin.|
| [`Product_Archive`](./classes/BigCommerce/Customizer/Sections/Product_Archive.md) | Customizer settings and controls for the Product Archive section.|
| [`Product_Category`](./classes/BigCommerce/Customizer/Sections/Product_Category.md) | Handles the customization of product category settings and controls.|
| [`Product_Single`](./classes/BigCommerce/Customizer/Sections/Product_Single.md) | Handles settings and constants related to the single product page in the BigCommerce integration.|





### \BigCommerce\Editor

#### Classes

| Class | Description |
|-------|-------------|
| [`Add_Products_Button`](./classes/BigCommerce/Editor/Add_Products_Button.md) | A class to render the &quot;Add Products&quot; button in the editor.|
| [`Editor_Dialog_Template`](./classes/BigCommerce/Editor/Editor_Dialog_Template.md) | A class that handles rendering the editor dialog template with product filtering options.|





### \BigCommerce\Editor\Gutenberg

#### Classes

| Class | Description |
|-------|-------------|
| [`Migrate_Blocks`](./classes/BigCommerce/Editor/Gutenberg/Migrate_Blocks.md) | Handles the migration of shortcodes to Gutenberg blocks in the editor. When a post is loaded in the<br />Gutenberg editor, this class manages the transition from legacy shortcodes to dynamic blocks<br />specific to the BigCommerce platform.|





### \BigCommerce\Editor\Gutenberg\Blocks

#### Classes

| Class | Description |
|-------|-------------|
| [`Account_Profile`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Account_Profile.md) | A block to display the current user&#039;s account profile.|
| [`Address_List`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Address_List.md) | A block to display the current user&#039;s addresses.|
| [`Cart`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Cart.md) | A block to display the current user&#039;s cart.|
| [`Checkout`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Checkout.md) | A block to display the checkout form.|
| [`Gift_Certificate_Balance`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Gift_Certificate_Balance.md) | A block to display the gift certificate balance form.|
| [`Gift_Certificate_Form`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Gift_Certificate_Form.md) | A block to display the gift certificate form.|
| [`Gutenberg_Block`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Gutenberg_Block.md) | A base class for creating Gutenberg blocks in BigCommerce.|
| [`Login_Form`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Login_Form.md) | A block to display the login form.|
| [`Order_History`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Order_History.md) | A block to display the current user&#039;s order history.|
| [`Product_Components`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Product_Components.md) | A block to display a given product&#039;s components.|
| [`Product_Reviews`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Product_Reviews.md) | A block to display a given product&#039;s reviews.|
| [`Products`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Products.md) | A block to add one or more products into the post content.|
| [`Registration_Form`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Registration_Form.md) | A block to display the registration form.|
| [`Shortcode_Block`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Shortcode_Block.md) | A Gutenberg Block that acts as a wrapper for a shortcode.|
| [`Wishlist`](./classes/BigCommerce/Editor/Gutenberg/Blocks/Wishlist.md) | A block to display the wishlist.|





### \BigCommerce\Exceptions

#### Classes

| Class | Description |
|-------|-------------|
| [`Channel_Not_Found_Exception`](./classes/BigCommerce/Exceptions/Channel_Not_Found_Exception.md) | Exception thrown when a channel cannot be found in the system.|
| [`Component_Not_Found_Exception`](./classes/BigCommerce/Exceptions/Component_Not_Found_Exception.md) | Exception thrown when a component cannot be found in the system.|
| [`No_Task_Found_Exception`](./classes/BigCommerce/Exceptions/No_Task_Found_Exception.md) | Exception thrown when a task cannot be found in the system.|
| [`Product_Not_Found_Exception`](./classes/BigCommerce/Exceptions/Product_Not_Found_Exception.md) | Exception thrown when a product cannot be found in the system.|





### \BigCommerce\Forms

#### Classes

| Class | Description |
|-------|-------------|
| [`Delete_Address_Handler`](./classes/BigCommerce/Forms/Delete_Address_Handler.md) | Handles the deletion of a customer&#039;s address from their account.|
| [`Error_Handler`](./classes/BigCommerce/Forms/Error_Handler.md) | Handles form error management, including storing and retrieving errors for redirection.|
| [`Form_Redirect`](./classes/BigCommerce/Forms/Form_Redirect.md) | Handles redirection after a form submission.|
| [`Messages`](./classes/BigCommerce/Forms/Messages.md) | Handles rendering of messages (success or error) above forms or within form submissions.|
| [`Product_Review_Handler`](./classes/BigCommerce/Forms/Product_Review_Handler.md) | |
| [`Purchase_Gift_Certificate_Handler`](./classes/BigCommerce/Forms/Purchase_Gift_Certificate_Handler.md) | Handles the submission and processing of gift certificate purchase forms.|
| [`Registration_Handler`](./classes/BigCommerce/Forms/Registration_Handler.md) | Handles user registration requests and form submissions for account creation.|
| [`Success_Handler`](./classes/BigCommerce/Forms/Success_Handler.md) | Handles the success of form submissions by storing a success message, form submission data,<br />and optionally redirecting the user to a specified URL or reloading the current page.|
| [`Switch_Currency_Handler`](./classes/BigCommerce/Forms/Switch_Currency_Handler.md) | Handles the logic for switching currencies in the BigCommerce cart and triggers success/error actions.|
| [`Update_Address_Handler`](./classes/BigCommerce/Forms/Update_Address_Handler.md) | Handles the updating and creation of customer addresses.|
| [`Update_Profile_Handler`](./classes/BigCommerce/Forms/Update_Profile_Handler.md) | Handles the profile update form submission process.|


#### Interfaces

| Interface | Description |
|-----------|-------------|
| [`Form_Handler`](./classes/BigCommerce/Forms/Form_Handler.md) | Interface for handling form submissions.|



### \BigCommerce\Functions




#### Functions

| Function | Description |
|----------|-------------|
| [`product_post_reviews`](./functions/BigCommerce/Functions/product_post_reviews().md) | Render reviews section for a product by post ID|
| [`product_reviews`](./functions/BigCommerce/Functions/product_reviews().md) | Render reviews section for a product by BigCommerce ID|


### \BigCommerce\Gift_Certificates

#### Classes

| Class | Description |
|-------|-------------|
| [`Sub_Nav`](./classes/BigCommerce/Gift_Certificates/Sub_Nav.md) | This class is responsible for adding a sub-navigation menu to the gift certificate and balance check pages.|





### \BigCommerce\GraphQL

#### Classes

| Class | Description |
|-------|-------------|
| [`BaseGQL`](./classes/BigCommerce/GraphQL/BaseGQL.md) | Handles interactions with the BigCommerce GraphQL API, including token management, making authenticated requests, and handling store-related information.|
| [`Customer_Query`](./classes/BigCommerce/GraphQL/Customer_Query.md) | Handles customer-related GraphQL queries and fragments.|
| [`GraphQL_Processor`](./classes/BigCommerce/GraphQL/GraphQL_Processor.md) | This class is responsible for handling GraphQL requests in the BigCommerce API context.|
| [`Product_Query`](./classes/BigCommerce/GraphQL/Product_Query.md) | Handle product query data and fragments.|
| [`Reviews_Query`](./classes/BigCommerce/GraphQL/Reviews_Query.md) | This class is responsible for constructing GraphQL queries related to product reviews.|
| [`Terms_Query`](./classes/BigCommerce/GraphQL/Terms_Query.md) | This class is responsible for constructing GraphQL queries related to terms,<br />including categories and brands. It provides methods to fetch term details<br />such as name, ID, and default image.|





### \BigCommerce\Import

#### Classes

| Class | Description |
|-------|-------------|
| [`Cache_Cleanup`](./classes/BigCommerce/Import/Cache_Cleanup.md) | Class Cache_Cleanup|
| [`Image_Importer`](./classes/BigCommerce/Import/Image_Importer.md) | Class Image_Importer|
| [`Import_Type`](./classes/BigCommerce/Import/Import_Type.md) | |
| [`Task_Definition`](./classes/BigCommerce/Import/Task_Definition.md) | |
| [`Task_Manager`](./classes/BigCommerce/Import/Task_Manager.md) | Class Task_Manager|

#### Traits

| Trait | Description |
|-------|-------------|
| [`No_Cache_Options`](./classes/BigCommerce/Import/No_Cache_Options.md) | Trait No_Cache_Options|

#### Interfaces

| Interface | Description |
|-----------|-------------|
| [`Import_Strategy`](./classes/BigCommerce/Import/Import_Strategy.md) | |



### \BigCommerce\Import\Importers\Products

#### Classes

| Class | Description |
|-------|-------------|
| [`Product_Builder`](./classes/BigCommerce/Import/Importers/Products/Product_Builder.md) | Responsible for constructing product-related data structures<br />during the import process for BigCommerce products.|
| [`Product_Creator`](./classes/BigCommerce/Import/Importers/Products/Product_Creator.md) | Handles the creation and saving of BigCommerce products into WordPress.|
| [`Product_Ignorer`](./classes/BigCommerce/Import/Importers/Products/Product_Ignorer.md) | Strategy for skipping a product during the import process.|
| [`Product_Importer`](./classes/BigCommerce/Import/Importers/Products/Product_Importer.md) | Handles the import of a product from BigCommerce to WordPress.|
| [`Product_Remover`](./classes/BigCommerce/Import/Importers/Products/Product_Remover.md) | Handles the removal of products from WordPress by matching them with their<br />corresponding BigCommerce product IDs and channel terms.|
| [`Product_Saver`](./classes/BigCommerce/Import/Importers/Products/Product_Saver.md) | Handles storing a product in the database, including saving product details,<br />taxonomy terms, images, and sending notifications after the product has been imported.|
| [`Product_Strategy_Factory`](./classes/BigCommerce/Import/Importers/Products/Product_Strategy_Factory.md) | Factory class for determining the appropriate import strategy for a product.|
| [`Product_Updater`](./classes/BigCommerce/Import/Importers/Products/Product_Updater.md) | Handles updating of products during the import process. It extends the Product_Saver class and overrides<br />the send_notifications method to send notifications when a product is updated.|





### \BigCommerce\Import\Importers\Terms

#### Classes

| Class | Description |
|-------|-------------|
| [`Term_Creator`](./classes/BigCommerce/Import/Importers/Terms/Term_Creator.md) | Class Term_Creator|
| [`Term_Ignorer`](./classes/BigCommerce/Import/Importers/Terms/Term_Ignorer.md) | Handles the logic for skipping the import of a term in the BigCommerce import process. This class implements<br />the Import_Strategy interface and provides a method for processing a term that should be ignored.|
| [`Term_Saver`](./classes/BigCommerce/Import/Importers/Terms/Term_Saver.md) | Provides functionality for saving terms into WordPress, including term data, term metadata,<br />and term images. This class implements the Import_Strategy interface, allowing it to be used<br />within an import process. It contains methods for handling terms in BigCommerce and saving them<br />in WordPress.|
| [`Term_Strategy_Factory`](./classes/BigCommerce/Import/Importers/Terms/Term_Strategy_Factory.md) | A factory class that determines the appropriate strategy for handling term imports,<br />such as creating, updating, or ignoring a term based on its existing data in WordPress.|
| [`Term_Updater`](./classes/BigCommerce/Import/Importers/Terms/Term_Updater.md) | This class is responsible for updating an existing term in WordPress with data from BigCommerce.|





### \BigCommerce\Import\Mappers

#### Classes

| Class | Description |
|-------|-------------|
| [`Brand_Mapper`](./classes/BigCommerce/Import/Mappers/Brand_Mapper.md) | This class is responsible for mapping the BigCommerce brand data to a WordPress term.|
| [`Product_Category_Mapper`](./classes/BigCommerce/Import/Mappers/Product_Category_Mapper.md) | This class is responsible for mapping the BigCommerce product category data to a WordPress term.|
| [`Term_Mapper`](./classes/BigCommerce/Import/Mappers/Term_Mapper.md) | This abstract class provides the base functionality for mapping BigCommerce terms to WordPress terms.|





### \BigCommerce\Import\Processors

#### Classes

| Class | Description |
|-------|-------------|
| [`Brand_Import`](./classes/BigCommerce/Import/Processors/Brand_Import.md) | This class handles the import process for BigCommerce brands. It extends the base Term_Import class<br />and provides the specific functionality for importing and updating brand terms in WordPress.|
| [`Brand_Purge`](./classes/BigCommerce/Import/Processors/Brand_Purge.md) | This class handles the process of purging (deleting) BigCommerce brand terms from WordPress.|
| [`Category_Import`](./classes/BigCommerce/Import/Processors/Category_Import.md) | Abstract class for processing term imports.|
| [`Category_Purge`](./classes/BigCommerce/Import/Processors/Category_Purge.md) | This class handles the process of purging product categories. It extends the<br />Term_Purge class and uses the CategoriesTrees trait to manage category trees.|
| [`Channel_Initializer`](./classes/BigCommerce/Import/Processors/Channel_Initializer.md) | Initializes a channel by linking it to the full product catalog.|
| [`Cleanup`](./classes/BigCommerce/Import/Processors/Cleanup.md) | Handles the cleanup process for BigCommerce imports, including purging product and user transients,<br />cleaning up queued tasks, and flushing cache related to products and customer groups.|
| [`Currencies`](./classes/BigCommerce/Import/Processors/Currencies.md) | This class handles fetching, processing, and storing currency information from BigCommerce.|
| [`Default_Customer_Group`](./classes/BigCommerce/Import/Processors/Default_Customer_Group.md) | |
| [`Deleted_Product_Marker`](./classes/BigCommerce/Import/Processors/Deleted_Product_Marker.md) | |
| [`Error_Handler`](./classes/BigCommerce/Import/Processors/Error_Handler.md) | |
| [`Headless`](./classes/BigCommerce/Import/Processors/Headless.md) | |
| [`Headless_Product_Processor`](./classes/BigCommerce/Import/Processors/Headless_Product_Processor.md) | |
| [`Image_Resizer`](./classes/BigCommerce/Import/Processors/Image_Resizer.md) | |
| [`Listing_Fetcher`](./classes/BigCommerce/Import/Processors/Listing_Fetcher.md) | |
| [`ProductCleanup`](./classes/BigCommerce/Import/Processors/ProductCleanup.md) | Purge BC products|
| [`Product_Data_Fetcher`](./classes/BigCommerce/Import/Processors/Product_Data_Fetcher.md) | |
| [`Queue_Runner`](./classes/BigCommerce/Import/Processors/Queue_Runner.md) | |
| [`Start_Import`](./classes/BigCommerce/Import/Processors/Start_Import.md) | |
| [`Store_Settings`](./classes/BigCommerce/Import/Processors/Store_Settings.md) | |
| [`Storefront_Processor`](./classes/BigCommerce/Import/Processors/Storefront_Processor.md) | |
| [`Term_Import`](./classes/BigCommerce/Import/Processors/Term_Import.md) | Abstract class for processing term imports.|
| [`Term_Purge`](./classes/BigCommerce/Import/Processors/Term_Purge.md) | Class Term_Purge|

#### Traits

| Trait | Description |
|-------|-------------|
| [`CategoriesTrees`](./classes/BigCommerce/Import/Processors/CategoriesTrees.md) | This trait provides methods for working with BigCommerce category trees.|

#### Interfaces

| Interface | Description |
|-----------|-------------|
| [`Import_Processor`](./classes/BigCommerce/Import/Processors/Import_Processor.md) | |



### \BigCommerce\Import\Runner

#### Classes

| Class | Description |
|-------|-------------|
| [`AsyncProcessing_Runner`](./classes/BigCommerce/Import/Runner/AsyncProcessing_Runner.md) | |
| [`CLI_Runner`](./classes/BigCommerce/Import/Runner/CLI_Runner.md) | |
| [`Cron_Monitor`](./classes/BigCommerce/Import/Runner/Cron_Monitor.md) | Class Cron_Monitor|
| [`Cron_Runner`](./classes/BigCommerce/Import/Runner/Cron_Runner.md) | |
| [`Cron_Scheduler`](./classes/BigCommerce/Import/Runner/Cron_Scheduler.md) | |
| [`Lock`](./classes/BigCommerce/Import/Runner/Lock.md) | |
| [`Lock_Monitor`](./classes/BigCommerce/Import/Runner/Lock_Monitor.md) | Class Lock_Monitor|
| [`Status`](./classes/BigCommerce/Import/Runner/Status.md) | |





### \BigCommerce\Logging

#### Classes

| Class | Description |
|-------|-------------|
| [`Error_Log`](./classes/BigCommerce/Logging/Error_Log.md) | Class Log|





### \BigCommerce\Manager

#### Classes

| Class | Description |
|-------|-------------|
| [`Channel_Update_Task`](./classes/BigCommerce/Manager/Channel_Update_Task.md) | |
| [`Manager`](./classes/BigCommerce/Manager/Manager.md) | |


#### Interfaces

| Interface | Description |
|-----------|-------------|
| [`Task`](./classes/BigCommerce/Manager/Task.md) | |



### \BigCommerce\Merchant

#### Classes

| Class | Description |
|-------|-------------|
| [`Account_Status`](./classes/BigCommerce/Merchant/Account_Status.md) | |
| [`Connect_Account`](./classes/BigCommerce/Merchant/Connect_Account.md) | |
| [`Create_Account`](./classes/BigCommerce/Merchant/Create_Account.md) | |
| [`Onboarding_Api`](./classes/BigCommerce/Merchant/Onboarding_Api.md) | |
| [`Setup_Status`](./classes/BigCommerce/Merchant/Setup_Status.md) | Class Setup_Status|





### \BigCommerce\Merchant\Models

#### Classes

| Class | Description |
|-------|-------------|
| [`Account_Contact`](./classes/BigCommerce/Merchant/Models/Account_Contact.md) | Class Account_Contact|
| [`Connect_Account_Request`](./classes/BigCommerce/Merchant/Models/Connect_Account_Request.md) | |
| [`Create_Account_Request`](./classes/BigCommerce/Merchant/Models/Create_Account_Request.md) | |
| [`Customer_Login_Request`](./classes/BigCommerce/Merchant/Models/Customer_Login_Request.md) | |





### \BigCommerce\Meta_Boxes

#### Classes

| Class | Description |
|-------|-------------|
| [`Meta_Box`](./classes/BigCommerce/Meta_Boxes/Meta_Box.md) | |
| [`Post_Meta_Box`](./classes/BigCommerce/Meta_Boxes/Post_Meta_Box.md) | |





### \BigCommerce\Nav_Menu

#### Classes

| Class | Description |
|-------|-------------|
| [`Dynamic_Menu_Items`](./classes/BigCommerce/Nav_Menu/Dynamic_Menu_Items.md) | |
| [`Nav_Items_Customizer`](./classes/BigCommerce/Nav_Menu/Nav_Items_Customizer.md) | Responsible for adding the BigCommerce nav items<br />into the theme customizer|
| [`Nav_Items_Meta_Box`](./classes/BigCommerce/Nav_Menu/Nav_Items_Meta_Box.md) | Responsible for handling the BigCommerce menu items<br />in the nav menu admin|





### \BigCommerce\Pages

#### Classes

| Class | Description |
|-------|-------------|
| [`Account_Page`](./classes/BigCommerce/Pages/Account_Page.md) | |
| [`Address_Page`](./classes/BigCommerce/Pages/Address_Page.md) | |
| [`Cart_Page`](./classes/BigCommerce/Pages/Cart_Page.md) | |
| [`Check_Balance_Page`](./classes/BigCommerce/Pages/Check_Balance_Page.md) | |
| [`Checkout_Complete_Page`](./classes/BigCommerce/Pages/Checkout_Complete_Page.md) | |
| [`Checkout_Page`](./classes/BigCommerce/Pages/Checkout_Page.md) | |
| [`Gift_Certificate_Page`](./classes/BigCommerce/Pages/Gift_Certificate_Page.md) | |
| [`Login_Page`](./classes/BigCommerce/Pages/Login_Page.md) | |
| [`Orders_Page`](./classes/BigCommerce/Pages/Orders_Page.md) | |
| [`Registration_Page`](./classes/BigCommerce/Pages/Registration_Page.md) | |
| [`Required_Page`](./classes/BigCommerce/Pages/Required_Page.md) | |
| [`Shipping_Returns_Page`](./classes/BigCommerce/Pages/Shipping_Returns_Page.md) | |
| [`Wishlist_Page`](./classes/BigCommerce/Pages/Wishlist_Page.md) | |





### \BigCommerce\Post_Types

#### Classes

| Class | Description |
|-------|-------------|
| [`Post_Type_Config`](./classes/BigCommerce/Post_Types/Post_Type_Config.md) | |





### \BigCommerce\Post_Types\Product

#### Classes

| Class | Description |
|-------|-------------|
| [`Admin_List`](./classes/BigCommerce/Post_Types/Product/Admin_List.md) | Handles extra columns for the BigCommerce Products post type|
| [`Admin_UI`](./classes/BigCommerce/Post_Types/Product/Admin_UI.md) | |
| [`Channel_Indicator`](./classes/BigCommerce/Post_Types/Product/Channel_Indicator.md) | Class Channel_Indicator|
| [`Channel_Sync`](./classes/BigCommerce/Post_Types/Product/Channel_Sync.md) | Class Channel_Sync|
| [`Config`](./classes/BigCommerce/Post_Types/Product/Config.md) | |
| [`Deletion`](./classes/BigCommerce/Post_Types/Product/Deletion.md) | |
| [`Product`](./classes/BigCommerce/Post_Types/Product/Product.md) | |
| [`Query`](./classes/BigCommerce/Post_Types/Product/Query.md) | Handles custom BigCommerce product queries in WordPress.|
| [`Query_Mapper`](./classes/BigCommerce/Post_Types/Product/Query_Mapper.md) | |
| [`Reset_Listing`](./classes/BigCommerce/Post_Types/Product/Reset_Listing.md) | Class Reset_Listing|
| [`Seo`](./classes/BigCommerce/Post_Types/Product/Seo.md) | Class Seo|
| [`Single_Product_Sync`](./classes/BigCommerce/Post_Types/Product/Single_Product_Sync.md) | Class Single_Product_Sync|
| [`Store_Links`](./classes/BigCommerce/Post_Types/Product/Store_Links.md) | |
| [`Unique_Slug_Filter`](./classes/BigCommerce/Post_Types/Product/Unique_Slug_Filter.md) | Class Unique_Slug_Filter|
| [`Unsupported_Products`](./classes/BigCommerce/Post_Types/Product/Unsupported_Products.md) | |
| [`WPGraph_Config`](./classes/BigCommerce/Post_Types/Product/WPGraph_Config.md) | |
| [`WPGraph_Product`](./classes/BigCommerce/Post_Types/Product/WPGraph_Product.md) | |





### \BigCommerce\Post_Types\Queue_Task

#### Classes

| Class | Description |
|-------|-------------|
| [`Config`](./classes/BigCommerce/Post_Types/Queue_Task/Config.md) | |
| [`Queue_Task`](./classes/BigCommerce/Post_Types/Queue_Task/Queue_Task.md) | |





### \BigCommerce\Post_Types\Sync_Log

#### Classes

| Class | Description |
|-------|-------------|
| [`Config`](./classes/BigCommerce/Post_Types/Sync_Log/Config.md) | |
| [`Sync_Log`](./classes/BigCommerce/Post_Types/Sync_Log/Sync_Log.md) | |





### \BigCommerce\Proxy

#### Classes

| Class | Description |
|-------|-------------|
| [`AMP_Cart_Controller`](./classes/BigCommerce/Proxy/AMP_Cart_Controller.md) | AMP_Cart_Controller class|
| [`Proxy_Cache`](./classes/BigCommerce/Proxy/Proxy_Cache.md) | Proxy_Cache class|
| [`Proxy_Controller`](./classes/BigCommerce/Proxy/Proxy_Controller.md) | Proxy_Controller class|





### \BigCommerce\Rest

#### Classes

| Class | Description |
|-------|-------------|
| [`Cart_Controller`](./classes/BigCommerce/Rest/Cart_Controller.md) | |
| [`Coupon_Code_Controller`](./classes/BigCommerce/Rest/Coupon_Code_Controller.md) | |
| [`Orders_Shortcode_Controller`](./classes/BigCommerce/Rest/Orders_Shortcode_Controller.md) | |
| [`Pricing_Controller`](./classes/BigCommerce/Rest/Pricing_Controller.md) | |
| [`Product_Component_Shortcode_Controller`](./classes/BigCommerce/Rest/Product_Component_Shortcode_Controller.md) | |
| [`Products_Controller`](./classes/BigCommerce/Rest/Products_Controller.md) | Class Products_Controller|
| [`Rest_Controller`](./classes/BigCommerce/Rest/Rest_Controller.md) | |
| [`Reviews_Listing_Controller`](./classes/BigCommerce/Rest/Reviews_Listing_Controller.md) | |
| [`Shipping_Controller`](./classes/BigCommerce/Rest/Shipping_Controller.md) | |
| [`Shortcode_Controller`](./classes/BigCommerce/Rest/Shortcode_Controller.md) | Class Products_Controller|
| [`Storefront_Controller`](./classes/BigCommerce/Rest/Storefront_Controller.md) | |
| [`Terms_Controller`](./classes/BigCommerce/Rest/Terms_Controller.md) | |





### \BigCommerce\Reviews

#### Classes

| Class | Description |
|-------|-------------|
| [`Product_Update_Listener`](./classes/BigCommerce/Reviews/Product_Update_Listener.md) | Class Product_Update_Listener|
| [`Review_Builder`](./classes/BigCommerce/Reviews/Review_Builder.md) | |
| [`Review_Cache`](./classes/BigCommerce/Reviews/Review_Cache.md) | Class Review_Cache|
| [`Review_Fetcher`](./classes/BigCommerce/Reviews/Review_Fetcher.md) | |





### \BigCommerce\Rewrites

#### Classes

| Class | Description |
|-------|-------------|
| [`Action_Endpoint`](./classes/BigCommerce/Rewrites/Action_Endpoint.md) | |
| [`Flusher`](./classes/BigCommerce/Rewrites/Flusher.md) | Handles flushing and scheduling of WordPress rewrite rules for the BigCommerce plugin.|





### \BigCommerce\Schema

#### Classes

| Class | Description |
|-------|-------------|
| [`Queue_Table`](./classes/BigCommerce/Schema/Queue_Table.md) | Class Queue_Table|
| [`Reviews_Table`](./classes/BigCommerce/Schema/Reviews_Table.md) | Class Reviews_Table|
| [`Schema`](./classes/BigCommerce/Schema/Schema.md) | |
| [`Table_Maker`](./classes/BigCommerce/Schema/Table_Maker.md) | Class Table_Maker|
| [`User_Roles`](./classes/BigCommerce/Schema/User_Roles.md) | |





### \BigCommerce\Settings

#### Classes

| Class | Description |
|-------|-------------|
| [`Abort_Import`](./classes/BigCommerce/Settings/Abort_Import.md) | |
| [`Connection_Status`](./classes/BigCommerce/Settings/Connection_Status.md) | |
| [`Flush_Cache`](./classes/BigCommerce/Settings/Flush_Cache.md) | |
| [`Import_Now`](./classes/BigCommerce/Settings/Import_Now.md) | |
| [`Import_Status`](./classes/BigCommerce/Settings/Import_Status.md) | Class Import_Status|
| [`Onboarding_Progress`](./classes/BigCommerce/Settings/Onboarding_Progress.md) | |
| [`Onboarding_Videos`](./classes/BigCommerce/Settings/Onboarding_Videos.md) | |
| [`Site_URL_Sync`](./classes/BigCommerce/Settings/Site_URL_Sync.md) | |
| [`Start_Over`](./classes/BigCommerce/Settings/Start_Over.md) | Class Start_Over|





### \BigCommerce\Settings\Screens

#### Classes

| Class | Description |
|-------|-------------|
| [`Abstract_Screen`](./classes/BigCommerce/Settings/Screens/Abstract_Screen.md) | Abstract base class for managing plugin settings screens.|
| [`Api_Credentials_Screen`](./classes/BigCommerce/Settings/Screens/Api_Credentials_Screen.md) | Abstract base class for managing plugin settings screens.|
| [`Connect_Channel_Screen`](./classes/BigCommerce/Settings/Screens/Connect_Channel_Screen.md) | Abstract base class for managing plugin settings screens.|
| [`Create_Account_Screen`](./classes/BigCommerce/Settings/Screens/Create_Account_Screen.md) | Abstract base class for managing plugin settings screens.|
| [`Nav_Menu_Screen`](./classes/BigCommerce/Settings/Screens/Nav_Menu_Screen.md) | Abstract base class for managing plugin settings screens.|
| [`Onboarding_Complete_Screen`](./classes/BigCommerce/Settings/Screens/Onboarding_Complete_Screen.md) | Abstract base class for managing plugin settings screens.|
| [`Onboarding_Screen`](./classes/BigCommerce/Settings/Screens/Onboarding_Screen.md) | Abstract base class for managing plugin settings screens.|
| [`Pending_Account_Screen`](./classes/BigCommerce/Settings/Screens/Pending_Account_Screen.md) | Abstract base class for managing plugin settings screens.|
| [`Resources_Screen`](./classes/BigCommerce/Settings/Screens/Resources_Screen.md) | Abstract base class for managing plugin settings screens.|
| [`Settings_Screen`](./classes/BigCommerce/Settings/Screens/Settings_Screen.md) | Abstract base class for managing plugin settings screens.|
| [`Store_Type_Screen`](./classes/BigCommerce/Settings/Screens/Store_Type_Screen.md) | Class Store_Type_Screen|
| [`Welcome_Screen`](./classes/BigCommerce/Settings/Screens/Welcome_Screen.md) | Abstract base class for managing plugin settings screens.|





### \BigCommerce\Settings\Sections

#### Classes

| Class | Description |
|-------|-------------|
| [`Account_Settings`](./classes/BigCommerce/Settings/Sections/Account_Settings.md) | |
| [`Analytics`](./classes/BigCommerce/Settings/Sections/Analytics.md) | |
| [`Api_Credentials`](./classes/BigCommerce/Settings/Sections/Api_Credentials.md) | |
| [`Cart`](./classes/BigCommerce/Settings/Sections/Cart.md) | |
| [`Channel_Select`](./classes/BigCommerce/Settings/Sections/Channel_Select.md) | |
| [`Channels`](./classes/BigCommerce/Settings/Sections/Channels.md) | Class Channels|
| [`Currency`](./classes/BigCommerce/Settings/Sections/Currency.md) | |
| [`Gift_Certificates`](./classes/BigCommerce/Settings/Sections/Gift_Certificates.md) | |
| [`Import`](./classes/BigCommerce/Settings/Sections/Import.md) | |
| [`Nav_Menu_Options`](./classes/BigCommerce/Settings/Sections/Nav_Menu_Options.md) | |
| [`New_Account_Section`](./classes/BigCommerce/Settings/Sections/New_Account_Section.md) | |
| [`Next_Steps`](./classes/BigCommerce/Settings/Sections/Next_Steps.md) | Class Next_Steps|
| [`Onboarding_Import_Settings`](./classes/BigCommerce/Settings/Sections/Onboarding_Import_Settings.md) | |
| [`Reviews`](./classes/BigCommerce/Settings/Sections/Reviews.md) | |
| [`Settings_Section`](./classes/BigCommerce/Settings/Sections/Settings_Section.md) | |
| [`Troubleshooting_Diagnostics`](./classes/BigCommerce/Settings/Sections/Troubleshooting_Diagnostics.md) | Class Troubleshooting_Diagnostics|
| [`Units`](./classes/BigCommerce/Settings/Sections/Units.md) | Class Units|
| [`Wishlists`](./classes/BigCommerce/Settings/Sections/Wishlists.md) | Class Wishlists|

#### Traits

| Trait | Description |
|-------|-------------|
| [`Images`](./classes/BigCommerce/Settings/Sections/Images.md) | |
| [`ImportType`](./classes/BigCommerce/Settings/Sections/ImportType.md) | |
| [`Webhooks`](./classes/BigCommerce/Settings/Sections/Webhooks.md) | |
| [`WithPages`](./classes/BigCommerce/Settings/Sections/WithPages.md) | |




### \BigCommerce\Shortcodes

#### Classes

| Class | Description |
|-------|-------------|
| [`Account_Profile`](./classes/BigCommerce/Shortcodes/Account_Profile.md) | |
| [`Address_List`](./classes/BigCommerce/Shortcodes/Address_List.md) | |
| [`Cart`](./classes/BigCommerce/Shortcodes/Cart.md) | |
| [`Checkout`](./classes/BigCommerce/Shortcodes/Checkout.md) | |
| [`Gift_Certificate_Balance`](./classes/BigCommerce/Shortcodes/Gift_Certificate_Balance.md) | |
| [`Gift_Certificate_Form`](./classes/BigCommerce/Shortcodes/Gift_Certificate_Form.md) | |
| [`Login_Form`](./classes/BigCommerce/Shortcodes/Login_Form.md) | |
| [`Order_History`](./classes/BigCommerce/Shortcodes/Order_History.md) | Provides a shortcode to display the order history for logged-in users.|
| [`Product_Components`](./classes/BigCommerce/Shortcodes/Product_Components.md) | |
| [`Product_Reviews`](./classes/BigCommerce/Shortcodes/Product_Reviews.md) | |
| [`Products`](./classes/BigCommerce/Shortcodes/Products.md) | |
| [`Registration_Form`](./classes/BigCommerce/Shortcodes/Registration_Form.md) | |
| [`Wishlist`](./classes/BigCommerce/Shortcodes/Wishlist.md) | |


#### Interfaces

| Interface | Description |
|-----------|-------------|
| [`Shortcode`](./classes/BigCommerce/Shortcodes/Shortcode.md) | |



### \BigCommerce\Taxonomies

#### Classes

| Class | Description |
|-------|-------------|
| [`Taxonomy_Config`](./classes/BigCommerce/Taxonomies/Taxonomy_Config.md) | |





### \BigCommerce\Taxonomies\Availability

#### Classes

| Class | Description |
|-------|-------------|
| [`Availability`](./classes/BigCommerce/Taxonomies/Availability/Availability.md) | |
| [`Config`](./classes/BigCommerce/Taxonomies/Availability/Config.md) | |





### \BigCommerce\Taxonomies\Brand

#### Classes

| Class | Description |
|-------|-------------|
| [`Brand`](./classes/BigCommerce/Taxonomies/Brand/Brand.md) | |
| [`Config`](./classes/BigCommerce/Taxonomies/Brand/Config.md) | |





### \BigCommerce\Taxonomies\Channel

#### Classes

| Class | Description |
|-------|-------------|
| [`Admin_Products_Filter`](./classes/BigCommerce/Taxonomies/Channel/Admin_Products_Filter.md) | Class Admin_Products_Filter|
| [`BC_Status`](./classes/BigCommerce/Taxonomies/Channel/BC_Status.md) | |
| [`Channel`](./classes/BigCommerce/Taxonomies/Channel/Channel.md) | |
| [`Channel_Connector`](./classes/BigCommerce/Taxonomies/Channel/Channel_Connector.md) | Class Channel_Connector|
| [`Channel_Synchronizer`](./classes/BigCommerce/Taxonomies/Channel/Channel_Synchronizer.md) | Class Channel_Synchronizer|
| [`Config`](./classes/BigCommerce/Taxonomies/Channel/Config.md) | |
| [`Connections`](./classes/BigCommerce/Taxonomies/Channel/Connections.md) | |
| [`Currency_Filter`](./classes/BigCommerce/Taxonomies/Channel/Currency_Filter.md) | |
| [`Query_Filter`](./classes/BigCommerce/Taxonomies/Channel/Query_Filter.md) | Class Query_Filter|
| [`Routes`](./classes/BigCommerce/Taxonomies/Channel/Routes.md) | Class Routes|





### \BigCommerce\Taxonomies\Condition

#### Classes

| Class | Description |
|-------|-------------|
| [`Condition`](./classes/BigCommerce/Taxonomies/Condition/Condition.md) | |
| [`Config`](./classes/BigCommerce/Taxonomies/Condition/Config.md) | |





### \BigCommerce\Taxonomies\Flag

#### Classes

| Class | Description |
|-------|-------------|
| [`Config`](./classes/BigCommerce/Taxonomies/Flag/Config.md) | |
| [`Flag`](./classes/BigCommerce/Taxonomies/Flag/Flag.md) | |





### \BigCommerce\Taxonomies\Product_Category

#### Classes

| Class | Description |
|-------|-------------|
| [`Config`](./classes/BigCommerce/Taxonomies/Product_Category/Config.md) | |
| [`Group_Filtered_Terms`](./classes/BigCommerce/Taxonomies/Product_Category/Group_Filtered_Terms.md) | |
| [`Product_Category`](./classes/BigCommerce/Taxonomies/Product_Category/Product_Category.md) | |
| [`Query_Filter`](./classes/BigCommerce/Taxonomies/Product_Category/Query_Filter.md) | |





### \BigCommerce\Taxonomies\Product_Type

#### Classes

| Class | Description |
|-------|-------------|
| [`Config`](./classes/BigCommerce/Taxonomies/Product_Type/Config.md) | |
| [`Product_Type`](./classes/BigCommerce/Taxonomies/Product_Type/Product_Type.md) | |





### \BigCommerce\Templates

#### Classes

| Class | Description |
|-------|-------------|
| [`Address_Actions`](./classes/BigCommerce/Templates/Address_Actions.md) | |
| [`Address_Delete`](./classes/BigCommerce/Templates/Address_Delete.md) | |
| [`Address_Form`](./classes/BigCommerce/Templates/Address_Form.md) | |
| [`Address_Formatted`](./classes/BigCommerce/Templates/Address_Formatted.md) | |
| [`Address_List`](./classes/BigCommerce/Templates/Address_List.md) | |
| [`Address_New`](./classes/BigCommerce/Templates/Address_New.md) | |
| [`Amp_Cart_Actions`](./classes/BigCommerce/Templates/Amp_Cart_Actions.md) | Amp_Cart_Actions class|
| [`Amp_Cart_Items`](./classes/BigCommerce/Templates/Amp_Cart_Items.md) | Amp_Cart_Items class|
| [`Amp_Cart_Summary`](./classes/BigCommerce/Templates/Amp_Cart_Summary.md) | Amp_Cart_Summary class|
| [`Body_Classes`](./classes/BigCommerce/Templates/Body_Classes.md) | |
| [`Cart`](./classes/BigCommerce/Templates/Cart.md) | |
| [`Cart_Action_Checkout`](./classes/BigCommerce/Templates/Cart_Action_Checkout.md) | |
| [`Cart_Action_View`](./classes/BigCommerce/Templates/Cart_Action_View.md) | |
| [`Cart_Actions`](./classes/BigCommerce/Templates/Cart_Actions.md) | |
| [`Cart_Coupon_Code`](./classes/BigCommerce/Templates/Cart_Coupon_Code.md) | |
| [`Cart_Empty`](./classes/BigCommerce/Templates/Cart_Empty.md) | |
| [`Cart_Error_Message`](./classes/BigCommerce/Templates/Cart_Error_Message.md) | |
| [`Cart_Footer`](./classes/BigCommerce/Templates/Cart_Footer.md) | |
| [`Cart_Header`](./classes/BigCommerce/Templates/Cart_Header.md) | |
| [`Cart_Items`](./classes/BigCommerce/Templates/Cart_Items.md) | |
| [`Cart_Summary`](./classes/BigCommerce/Templates/Cart_Summary.md) | |
| [`Controller`](./classes/BigCommerce/Templates/Controller.md) | |
| [`Controller_Factory`](./classes/BigCommerce/Templates/Controller_Factory.md) | |
| [`Currency_Switcher_Form`](./classes/BigCommerce/Templates/Currency_Switcher_Form.md) | |
| [`Fallback_Image`](./classes/BigCommerce/Templates/Fallback_Image.md) | |
| [`Form_Controller`](./classes/BigCommerce/Templates/Form_Controller.md) | |
| [`Gift_Certificate_Balance_Form`](./classes/BigCommerce/Templates/Gift_Certificate_Balance_Form.md) | |
| [`Gift_Certificate_Balance_Page`](./classes/BigCommerce/Templates/Gift_Certificate_Balance_Page.md) | |
| [`Gift_Certificate_Balance_Response`](./classes/BigCommerce/Templates/Gift_Certificate_Balance_Response.md) | |
| [`Gift_Certificate_Form`](./classes/BigCommerce/Templates/Gift_Certificate_Form.md) | |
| [`Gift_Certificate_Page`](./classes/BigCommerce/Templates/Gift_Certificate_Page.md) | |
| [`Gift_Certificate_Redemption_Instructions`](./classes/BigCommerce/Templates/Gift_Certificate_Redemption_Instructions.md) | |
| [`Inventory_Level`](./classes/BigCommerce/Templates/Inventory_Level.md) | |
| [`Linked_Product_Featured_Image`](./classes/BigCommerce/Templates/Linked_Product_Featured_Image.md) | |
| [`Login_Form`](./classes/BigCommerce/Templates/Login_Form.md) | |
| [`Lost_Password_Form`](./classes/BigCommerce/Templates/Lost_Password_Form.md) | |
| [`Message`](./classes/BigCommerce/Templates/Message.md) | |
| [`Message_Group`](./classes/BigCommerce/Templates/Message_Group.md) | |
| [`Mini_Cart`](./classes/BigCommerce/Templates/Mini_Cart.md) | |
| [`Mini_Cart_Actions`](./classes/BigCommerce/Templates/Mini_Cart_Actions.md) | |
| [`Mini_Cart_Footer`](./classes/BigCommerce/Templates/Mini_Cart_Footer.md) | |
| [`Mini_Cart_Header`](./classes/BigCommerce/Templates/Mini_Cart_Header.md) | |
| [`Mini_Cart_Items`](./classes/BigCommerce/Templates/Mini_Cart_Items.md) | |
| [`Mini_Cart_Summary`](./classes/BigCommerce/Templates/Mini_Cart_Summary.md) | |
| [`No_Results`](./classes/BigCommerce/Templates/No_Results.md) | |
| [`Order_Details`](./classes/BigCommerce/Templates/Order_Details.md) | |
| [`Order_History`](./classes/BigCommerce/Templates/Order_History.md) | |
| [`Order_Not_Found`](./classes/BigCommerce/Templates/Order_Not_Found.md) | |
| [`Order_Product`](./classes/BigCommerce/Templates/Order_Product.md) | |
| [`Order_Shipment`](./classes/BigCommerce/Templates/Order_Shipment.md) | |
| [`Order_Summary`](./classes/BigCommerce/Templates/Order_Summary.md) | |
| [`Orders_Shortcode_Pagination`](./classes/BigCommerce/Templates/Orders_Shortcode_Pagination.md) | |
| [`Page_Wrapper`](./classes/BigCommerce/Templates/Page_Wrapper.md) | |
| [`Product_Archive`](./classes/BigCommerce/Templates/Product_Archive.md) | |
| [`Product_Brand`](./classes/BigCommerce/Templates/Product_Brand.md) | |
| [`Product_Card`](./classes/BigCommerce/Templates/Product_Card.md) | |
| [`Product_Card_Preview`](./classes/BigCommerce/Templates/Product_Card_Preview.md) | |
| [`Product_Condition`](./classes/BigCommerce/Templates/Product_Condition.md) | |
| [`Product_Description`](./classes/BigCommerce/Templates/Product_Description.md) | |
| [`Product_Featured_Image`](./classes/BigCommerce/Templates/Product_Featured_Image.md) | |
| [`Product_Form`](./classes/BigCommerce/Templates/Product_Form.md) | |
| [`Product_Form_Preview`](./classes/BigCommerce/Templates/Product_Form_Preview.md) | A specialized version of the product form that disables purchase functionality.|
| [`Product_Gallery`](./classes/BigCommerce/Templates/Product_Gallery.md) | |
| [`Product_Hidden_Price`](./classes/BigCommerce/Templates/Product_Hidden_Price.md) | |
| [`Product_Not_Available`](./classes/BigCommerce/Templates/Product_Not_Available.md) | |
| [`Product_Options`](./classes/BigCommerce/Templates/Product_Options.md) | |
| [`Product_Price`](./classes/BigCommerce/Templates/Product_Price.md) | |
| [`Product_Quick_View`](./classes/BigCommerce/Templates/Product_Quick_View.md) | |
| [`Product_Rating`](./classes/BigCommerce/Templates/Product_Rating.md) | |
| [`Product_Reviews`](./classes/BigCommerce/Templates/Product_Reviews.md) | |
| [`Product_Shortcode_Grid`](./classes/BigCommerce/Templates/Product_Shortcode_Grid.md) | |
| [`Product_Shortcode_Pagination`](./classes/BigCommerce/Templates/Product_Shortcode_Pagination.md) | |
| [`Product_Shortcode_Single`](./classes/BigCommerce/Templates/Product_Shortcode_Single.md) | |
| [`Product_Shortcode_Single_Preview`](./classes/BigCommerce/Templates/Product_Shortcode_Single_Preview.md) | |
| [`Product_Single`](./classes/BigCommerce/Templates/Product_Single.md) | |
| [`Product_Sku`](./classes/BigCommerce/Templates/Product_Sku.md) | |
| [`Product_Specs`](./classes/BigCommerce/Templates/Product_Specs.md) | |
| [`Product_Title`](./classes/BigCommerce/Templates/Product_Title.md) | |
| [`Profile_Form`](./classes/BigCommerce/Templates/Profile_Form.md) | |
| [`Quick_View_Image`](./classes/BigCommerce/Templates/Quick_View_Image.md) | |
| [`Refinement_Box`](./classes/BigCommerce/Templates/Refinement_Box.md) | |
| [`Refinery`](./classes/BigCommerce/Templates/Refinery.md) | |
| [`Registration_Form`](./classes/BigCommerce/Templates/Registration_Form.md) | |
| [`Related_Product`](./classes/BigCommerce/Templates/Related_Product.md) | |
| [`Related_Products_Grid`](./classes/BigCommerce/Templates/Related_Products_Grid.md) | |
| [`Review_Form`](./classes/BigCommerce/Templates/Review_Form.md) | |
| [`Review_List`](./classes/BigCommerce/Templates/Review_List.md) | |
| [`Review_List_Pagination`](./classes/BigCommerce/Templates/Review_List_Pagination.md) | |
| [`Review_Single`](./classes/BigCommerce/Templates/Review_Single.md) | |
| [`Search_Box`](./classes/BigCommerce/Templates/Search_Box.md) | |
| [`Shipping_Info_Button`](./classes/BigCommerce/Templates/Shipping_Info_Button.md) | |
| [`Shipping_Methods`](./classes/BigCommerce/Templates/Shipping_Methods.md) | |
| [`Shipping_Zones_Dropdown`](./classes/BigCommerce/Templates/Shipping_Zones_Dropdown.md) | |
| [`Sub_Nav_Links`](./classes/BigCommerce/Templates/Sub_Nav_Links.md) | |
| [`Template`](./classes/BigCommerce/Templates/Template.md) | |
| [`Template_Override`](./classes/BigCommerce/Templates/Template_Override.md) | Class Template_Override|
| [`View_Product_Button`](./classes/BigCommerce/Templates/View_Product_Button.md) | |
| [`Wishlist_Add_Item`](./classes/BigCommerce/Templates/Wishlist_Add_Item.md) | |
| [`Wishlist_Create`](./classes/BigCommerce/Templates/Wishlist_Create.md) | |
| [`Wishlist_Delete`](./classes/BigCommerce/Templates/Wishlist_Delete.md) | |
| [`Wishlist_Detail`](./classes/BigCommerce/Templates/Wishlist_Detail.md) | |
| [`Wishlist_Detail_Breadcrumb`](./classes/BigCommerce/Templates/Wishlist_Detail_Breadcrumb.md) | |
| [`Wishlist_Detail_Header`](./classes/BigCommerce/Templates/Wishlist_Detail_Header.md) | |
| [`Wishlist_Detail_Share`](./classes/BigCommerce/Templates/Wishlist_Detail_Share.md) | |
| [`Wishlist_Edit`](./classes/BigCommerce/Templates/Wishlist_Edit.md) | |
| [`Wishlist_List`](./classes/BigCommerce/Templates/Wishlist_List.md) | |
| [`Wishlist_List_Row`](./classes/BigCommerce/Templates/Wishlist_List_Row.md) | |
| [`Wishlist_New_Button`](./classes/BigCommerce/Templates/Wishlist_New_Button.md) | |
| [`Wishlist_New_Link`](./classes/BigCommerce/Templates/Wishlist_New_Link.md) | Class Wishlist_New_Link|
| [`Wishlist_Not_Available`](./classes/BigCommerce/Templates/Wishlist_Not_Available.md) | |
| [`Wishlist_Product`](./classes/BigCommerce/Templates/Wishlist_Product.md) | Class Wishlist_Product|

#### Traits

| Trait | Description |
|-------|-------------|
| [`CDN_Images`](./classes/BigCommerce/Templates/CDN_Images.md) | |
| [`Product_TemplateTrait`](./classes/BigCommerce/Templates/Product_TemplateTrait.md) | |




### \BigCommerce\Templates\Option_Types

#### Classes

| Class | Description |
|-------|-------------|
| [`Option_Checkbox`](./classes/BigCommerce/Templates/Option_Types/Option_Checkbox.md) | |
| [`Option_Date`](./classes/BigCommerce/Templates/Option_Types/Option_Date.md) | |
| [`Option_Dropdown`](./classes/BigCommerce/Templates/Option_Types/Option_Dropdown.md) | |
| [`Option_Number`](./classes/BigCommerce/Templates/Option_Types/Option_Number.md) | |
| [`Option_Product_List`](./classes/BigCommerce/Templates/Option_Types/Option_Product_List.md) | |
| [`Option_Product_List_With_Images`](./classes/BigCommerce/Templates/Option_Types/Option_Product_List_With_Images.md) | |
| [`Option_Radios`](./classes/BigCommerce/Templates/Option_Types/Option_Radios.md) | |
| [`Option_Rectangles`](./classes/BigCommerce/Templates/Option_Types/Option_Rectangles.md) | |
| [`Option_Swatch`](./classes/BigCommerce/Templates/Option_Types/Option_Swatch.md) | |
| [`Option_Text`](./classes/BigCommerce/Templates/Option_Types/Option_Text.md) | |
| [`Option_Textarea`](./classes/BigCommerce/Templates/Option_Types/Option_Textarea.md) | |
| [`Option_Type`](./classes/BigCommerce/Templates/Option_Types/Option_Type.md) | |





### \BigCommerce\Util

#### Classes

| Class | Description |
|-------|-------------|
| [`Cart_Item_Iterator`](./classes/BigCommerce/Util/Cart_Item_Iterator.md) | |
| [`Kses`](./classes/BigCommerce/Util/Kses.md) | |





### \BigCommerce\Webhooks

#### Classes

| Class | Description |
|-------|-------------|
| [`Checkout_Complete_Webhook`](./classes/BigCommerce/Webhooks/Checkout_Complete_Webhook.md) | Class Checkout Complete Webhook|
| [`Status`](./classes/BigCommerce/Webhooks/Status.md) | Class Status|
| [`Webhook`](./classes/BigCommerce/Webhooks/Webhook.md) | Sets up a webhook in the BigCommerce API to send event-based requests to the WP site.|
| [`Webhook_Cron_Tasks`](./classes/BigCommerce/Webhooks/Webhook_Cron_Tasks.md) | Class Webhook_Cron_Tasks|
| [`Webhook_Listener`](./classes/BigCommerce/Webhooks/Webhook_Listener.md) | Class Webhook_Listener|
| [`Webhook_Versioning`](./classes/BigCommerce/Webhooks/Webhook_Versioning.md) | Class Webhook_Versioning|

#### Traits

| Trait | Description |
|-------|-------------|
| [`WebhookTrait`](./classes/BigCommerce/Webhooks/WebhookTrait.md) | |




### \BigCommerce\Webhooks\Customer

#### Classes

| Class | Description |
|-------|-------------|
| [`Customer_Channel_Updater`](./classes/BigCommerce/Webhooks/Customer/Customer_Channel_Updater.md) | |
| [`Customer_Channel_Webhook`](./classes/BigCommerce/Webhooks/Customer/Customer_Channel_Webhook.md) | Class Customer_Channel_Webhook|
| [`Customer_Create_Webhook`](./classes/BigCommerce/Webhooks/Customer/Customer_Create_Webhook.md) | Class Customer_Create_Webhook|
| [`Customer_Creator`](./classes/BigCommerce/Webhooks/Customer/Customer_Creator.md) | |
| [`Customer_Delete_Webhook`](./classes/BigCommerce/Webhooks/Customer/Customer_Delete_Webhook.md) | Class Product_Delete_Webhook|
| [`Customer_Deleter`](./classes/BigCommerce/Webhooks/Customer/Customer_Deleter.md) | |
| [`Customer_Saver`](./classes/BigCommerce/Webhooks/Customer/Customer_Saver.md) | |
| [`Customer_Update_Webhook`](./classes/BigCommerce/Webhooks/Customer/Customer_Update_Webhook.md) | Class Customer_Update_Webhook|
| [`Customer_Updater`](./classes/BigCommerce/Webhooks/Customer/Customer_Updater.md) | |





### \BigCommerce\Webhooks\Product

#### Classes

| Class | Description |
|-------|-------------|
| [`Channel_Updater`](./classes/BigCommerce/Webhooks/Product/Channel_Updater.md) | |
| [`Channels_Assign`](./classes/BigCommerce/Webhooks/Product/Channels_Assign.md) | |
| [`Channels_Currency_Update`](./classes/BigCommerce/Webhooks/Product/Channels_Currency_Update.md) | |
| [`Channels_Management_Webhook`](./classes/BigCommerce/Webhooks/Product/Channels_Management_Webhook.md) | Class Channels_Management_Webhook|
| [`Channels_Manager`](./classes/BigCommerce/Webhooks/Product/Channels_Manager.md) | |
| [`Channels_UnAssign`](./classes/BigCommerce/Webhooks/Product/Channels_UnAssign.md) | |
| [`Product_Create_Webhook`](./classes/BigCommerce/Webhooks/Product/Product_Create_Webhook.md) | Class Product_Create_Webhook|
| [`Product_Creator`](./classes/BigCommerce/Webhooks/Product/Product_Creator.md) | Handles the creation of a new product from BigCommerce via webhooks.|
| [`Product_Delete_Webhook`](./classes/BigCommerce/Webhooks/Product/Product_Delete_Webhook.md) | Class Product_Delete_Webhook|
| [`Product_Inventory_Update_Webhook`](./classes/BigCommerce/Webhooks/Product/Product_Inventory_Update_Webhook.md) | Class Product_Inventory_Update_Webhook|
| [`Product_Update_Webhook`](./classes/BigCommerce/Webhooks/Product/Product_Update_Webhook.md) | Class Product_Update_Webhook|
| [`Product_Updater`](./classes/BigCommerce/Webhooks/Product/Product_Updater.md) | Class Product_Updater|





### \BigCommerce\Widgets

#### Classes

| Class | Description |
|-------|-------------|
| [`Currency_Switcher_Widget`](./classes/BigCommerce/Widgets/Currency_Switcher_Widget.md) | Class Currency_Switcher_Widget|
| [`Mini_Cart_Widget`](./classes/BigCommerce/Widgets/Mini_Cart_Widget.md) | Class Product_Category_Widget|
| [`Product_Category_Widget`](./classes/BigCommerce/Widgets/Product_Category_Widget.md) | Class Product_Category_Widget|





***
> Automatically generated on 2024-12-13
