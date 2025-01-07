***

# Image_Sizes

Class Image_Sizes

Registers custom image sizes for the BigCommerce theme, providing predefined sizes
for product images, thumbnails, and category images. The version constant is incremented
when any changes are made to the image sizes list.

* Full name: `\BigCommerce\Assets\Theme\Image_Sizes`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`VERSION`|public|int|2|
|`STATE_META`|public|string|&#039;bigcommerce_sizing&#039;|
|`BC_THUMB`|public|string|&#039;bc-thumb&#039;|
|`BC_THUMB_LARGE`|public|string|&#039;bc-thumb-large&#039;|
|`BC_SMALL`|public|string|&#039;bc-small&#039;|
|`BC_MEDIUM`|public|string|&#039;bc-medium&#039;|
|`BC_EXTRA_MEDIUM`|public|string|&#039;bc-xmedium&#039;|
|`BC_LARGE`|public|string|&#039;bc-large&#039;|
|`BC_CATEGORY_IMAGE`|public|string|&#039;bc-category-image&#039;|


## Methods


### register_sizes

Registers custom image sizes with WordPress.

```php
public register_sizes(): void
```

This method loops through the defined image sizes and registers each one using
the `add_image_size` function. The sizes are registered when the theme is set up.










***


***
> Automatically generated on 2025-01-07
