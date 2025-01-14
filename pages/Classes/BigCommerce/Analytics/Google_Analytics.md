***

# Google_Analytics

Class Google_Analytics

Renders the Google Analytics tracking code on the site.

This class is responsible for injecting the Google Analytics tracking code into the
`<head>` section of the website. The tracking code is used to gather analytics
data about site visitors, including traffic and user behavior. The tracking code
is only added if a valid Google Analytics ID is set in the settings.

* Full name: `\BigCommerce\Analytics\Google_Analytics`




## Methods


### render_tracking_code

Renders the Google Analytics tracking code in the site's head section.

```php
public render_tracking_code(): void
```

This function retrieves the Google Analytics tracking ID from the site settings
and generates the necessary JavaScript code for integrating Google Analytics tracking.
The script is added to the `<head>` section of the webpage using the `wp_head` action hook.
If no Google Analytics ID is set, the function does nothing.










***


***
> Automatically generated on 2025-01-14
