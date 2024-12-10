***

# Facebook_Pixel

Class Facebook_Pixel

Renders the Facebook Pixel tracking code on the site.

This class is responsible for injecting the Facebook Pixel tracking code into the
`<head>` section of the website. The tracking code is used to track user interactions
for the purpose of running analytics and ad targeting on Facebook.
The tracking code is only added if a valid Facebook Pixel ID is set in the settings.

* Full name: `\BigCommerce\Analytics\Facebook_Pixel`




## Methods


### render_tracking_code

Renders the Facebook Pixel tracking code in the site's head section.

```php
public render_tracking_code(): void
```

This function retrieves the Facebook Pixel ID from the site settings and generates
the necessary JavaScript code for integrating Facebook Pixel tracking. The script is
added to the `<head>` section of the webpage using the `wp_head` action hook.
If no Facebook Pixel ID is set, the function does nothing.










***


***
> Automatically generated on 2024-12-10
