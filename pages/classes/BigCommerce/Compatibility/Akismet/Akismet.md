***

# Akismet

This class implements the Spam_Checker interface and uses the Akismet API to determine if a submission is considered spam.

It checks submissions against the Akismet service based on the provided details such as user IP, email, name, and referrer.

The `is_spam` method makes an HTTP request to the Akismet API, and if the submission is flagged as spam, it updates the Akismet spam count.
The Akismet API key must be set in WordPress options for the class to function.

Usage:
       $akismet = new Akismet();
       $result = $akismet->is_spam( $submission );

* Full name: `\BigCommerce\Compatibility\Akismet\Akismet`
* This class implements:
[`\BigCommerce\Compatibility\Spam_Checker`](../Spam_Checker.md)




## Methods


### is_spam

Checks whether a submission is flagged as spam by the Akismet service.

```php
public is_spam(array $submission): bool
```

This method sends the submission details to Akismet's API for spam checking. If the submission is flagged as spam,
the spam count in WordPress options is updated. It returns `true` if the submission is spam, otherwise `false`.






**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **array** | An associative array containing the submission data, including first name, last name, email, etc. |


**Return Value:**

Returns `true` if the submission is spam, otherwise `false`.




***

### get_query_string



```php
private get_query_string(mixed $submission): mixed
```








**Parameters:**

| Parameter | Type | Description |
|-----------|------|-------------|
| `$submission` | **mixed** |  |





***


***
> Automatically generated on 2024-12-10