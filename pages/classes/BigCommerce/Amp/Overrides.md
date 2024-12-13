***

# Overrides

Class Overrides

Provides custom AMP-specific overrides and modifications,
including handling image sources, enabling AMP buttons,
and defining allowed HTML tags for AMP templates.

* Full name: `\BigCommerce\Amp\Overrides`




## Methods


### add_amp_img_src

Add AMP image source.

```php
public add_amp_img_src(array $data, string $template): array
```

Adds `image_src` and `image_srcset` to the data passed to the product featured image template
for AMP compatibility.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$data` | **array** | Data to be sent to the template. |
| `$template` | **string** | Current template being rendered. |


**Return Value:**

Modified data array.




***

### amp_enable_button

Enable AMP button.

```php
public amp_enable_button(string $button, int $post_id): string
```

Dynamically enables the AMP submit button when a proper product variant is selected.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$button` | **string** | Original button HTML. |
| `$post_id` | **int** | ID of the current post or product. |


**Return Value:**

Modified button HTML.




***

### add_amp_redirect_headers

Add AMP redirect headers.

```php
public add_amp_redirect_headers(string $url): void
```

Adds necessary headers for AMP redirects and ensures proper URL formatting.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$url` | **string** | The URL to redirect to. |





***

### filter_fallback_image

Filter fallback image for AMP.

```php
public filter_fallback_image(): string
```

Returns a formatted AMP-compliant image placeholder.







**Return Value:**

AMP-compliant `<amp-img>` HTML for the fallback image.




***

### amp_kses_allowed_html

Customize allowed HTML tags for AMP context.

```php
public amp_kses_allowed_html(array $allowed_tags, string $context): array
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$allowed_tags` | **array** | Array of allowed HTML tags. |
| `$context` | **string** | Context for filtering. |


**Return Value:**

Modified array of allowed tags.




***


***
> Automatically generated on 2024-12-13
