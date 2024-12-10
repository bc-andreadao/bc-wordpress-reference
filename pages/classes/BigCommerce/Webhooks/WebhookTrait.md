***

# WebhookTrait





* Full name: `\BigCommerce\Webhooks\WebhookTrait`




## Methods


### product_webhooks_enabled

Is product webhooks are enabled

```php
public product_webhooks_enabled(): bool
```












***

### customer_webhooks_enabled

If customer webhooks are enabled

```php
public customer_webhooks_enabled(): bool
```












***

### maybe_skip_product_hooks

Should we skip the product hook or no

```php
public maybe_skip_product_hooks(string $hook = &#039;&#039;, false $hooks_enabled = false): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$hook` | **string** |  |
| `$hooks_enabled` | **false** |  |





***

### maybe_skip_customer_hooks

Should we skip the customer hook or no

```php
public maybe_skip_customer_hooks(string $hook = &#039;&#039;, false $hooks_enabled = false): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$hook` | **string** |  |
| `$hooks_enabled` | **false** |  |





***

### is_customer_webhook

Check if it is a customer webhook

```php
public is_customer_webhook(string $hook = &#039;&#039;): bool
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$hook` | **string** |  |





***

### get_customer_webhooks

Return list of customer webhooks

```php
public get_customer_webhooks(): array
```












***

***
> Automatically generated on 2024-12-10

