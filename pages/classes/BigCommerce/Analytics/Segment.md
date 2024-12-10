***

# Segment

Renders the Segment analytics tracking code on the site.

This class is responsible for injecting the Segment analytics tracking code into the
`<head>` section of the website. The code is used to collect data on user behavior,
page views, and other user interactions. The tracking code is only added if a valid
Segment key is set in the settings.

* Full name: `\BigCommerce\Analytics\Segment`




## Methods


### render_tracking_code

Renders the Segment analytics tracking code in the site's head section.

```php
public render_tracking_code(): void
```

This function retrieves the Segment tracking key and settings, and generates
the necessary JavaScript code for integrating Segment analytics tracking.
The script is added to the `<head>` section of the webpage using the `wp_head` action hook.
If no Segment key is set, the function does nothing.










***

### get_settings

Retrieves a list of the analytics settings.

```php
private get_settings(): object
```

This function collects the relevant analytics settings, including configurations
for Google Analytics and Facebook Pixel, and returns them in an object format.
These settings are then used to configure the Segment analytics integration.







**Return Value:**

The analytics settings object.




***


***
> Automatically generated on 2024-12-10
