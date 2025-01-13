***

# Sub_Nav

Class Sub_Nav

Responsible for rendering and saving profile settings, as well as managing the visibility of the sub-navigation menu
above the content for account-related pages.

* Full name: `\BigCommerce\Accounts\Sub_Nav`




## Methods


### add_subnav_above_content

Handle subnav visibility above the content

```php
public add_subnav_above_content(string $content): string
```

This filter is applied to the page content and will insert the sub-navigation
if the user is logged in and the page is part of the account-related pages.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$content` | **string** | The content of the page. |


**Return Value:**

Filtered content with subnav included if applicable.




***


***
> Automatically generated on 2025-01-13
