***

# Image_Importer

Class Image_Importer

Imports an image from a URL and attaches it to a post

* Full name: `\BigCommerce\Import\Image_Importer`


## Constants

| Constant | Visibility | Type | Value |
|:---------|:-----------|:-----|:------|
|`SOURCE_URL`|public| |&#039;bigcommerce_source_url&#039;|
|`URL_ZOOM`|public| |&#039;url_zoom&#039;|
|`URL_STD`|public| |&#039;url_standard&#039;|
|`URL_THUMB`|public| |&#039;url_thumbnail&#039;|
|`URL_TINY`|public| |&#039;url_tiny&#039;|
|`IMAGE_ALT`|public| |&#039;image_alt&#039;|
|`FULL_IMAGE_IMPORT`|public| |&#039;bigcommerce_allow_full_image_import&#039;|
|`CDN_IMAGE_IMPORT`|public| |&#039;bigcommerce_allow_cdn_image_import&#039;|
|`DISABLE_IMAGE_IMPORT`|public| |&#039;bigcommerce_disable_image_import&#039;|
|`MIMES`|public| |[IMAGETYPE_GIF =&gt; &#039;image/gif&#039;, IMAGETYPE_JPEG =&gt; &#039;image/jpg&#039;, IMAGETYPE_PNG =&gt; &#039;image/png&#039;, IMAGETYPE_SWF =&gt; &#039;image/swf&#039;, IMAGETYPE_PSD =&gt; &#039;image/psd&#039;, IMAGETYPE_BMP =&gt; &#039;image/bmp&#039;, IMAGETYPE_TIFF_II =&gt; &#039;image/tiff&#039;, IMAGETYPE_TIFF_MM =&gt; &#039;image/tiff&#039;, IMAGETYPE_JPC =&gt; &#039;image/jpc&#039;, IMAGETYPE_JP2 =&gt; &#039;image/jp2&#039;, IMAGETYPE_JPX =&gt; &#039;image/jpx&#039;, IMAGETYPE_JB2 =&gt; &#039;image/jb2&#039;, IMAGETYPE_SWC =&gt; &#039;image/swc&#039;, IMAGETYPE_IFF =&gt; &#039;image/iff&#039;, IMAGETYPE_WBMP =&gt; &#039;image/wbmp&#039;, IMAGETYPE_XBM =&gt; &#039;image/xbm&#039;, IMAGETYPE_ICO =&gt; &#039;image/ico&#039;]|


## Methods


### __construct



```php
public __construct(mixed $image_url, mixed $attach_to_post_id): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$image_url` | **mixed** |  |
| `$attach_to_post_id` | **mixed** |  |





***

### import



```php
public import(false $is_category = false): false|int|\WP_Error
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$is_category` | **false** |  |





***

### should_load_from_cdn

Check if images serving from BigCommerce CDN is enabled

```php
public static should_load_from_cdn(): bool
```



* This method is **static**.








***

### is_image_import_allowed

Check whether image import is enabled

```php
public static is_image_import_allowed(): bool
```



* This method is **static**.








***

### has_local_featured_image

Is featured image exists only on WP side

```php
public static has_local_featured_image(int $post_id): bool
```



* This method is **static**.




**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$post_id` | **int** |  |





***


***
> Automatically generated on 2024-12-10
