***

# Sub_Nav

This class is responsible for adding a sub-navigation menu to the gift certificate and balance check pages.

The sub-navigation is dynamically rendered above the page content based on certain conditions.

It listens for the `the_content` filter to insert the sub-navigation at the beginning of the page content.
The sub-navigation links are fetched from the Gift Certificate and Balance Check pages, and their display
can be customized via filters.

* Full name: `\BigCommerce\Gift_Certificates\Sub_Nav`




## Methods


### add_subnav_above_content

Filters the content of the page to add a sub-navigation menu above the content on gift certificate pages.

```php
public add_subnav_above_content(string $content): string
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$content` | **string** | The content of the page. |


**Return Value:**

The content with the sub-navigation added if the page is a gift certificate page.




***


***
> Automatically generated on 2024-12-10
