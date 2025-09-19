# Shopify Customer Privacy API Tag for Google Tag Manager Web

The **Shopify Customer Privacy API Tag** for Google Tag Manager Web allows you to set customer consent choices on your Shopify store by interacting with Shopify's [Customer Privacy API](https://shopify.dev/docs/api/customer-privacy). The tag is useful when your consent banner does not integrate with Shopify Consent Management.

It helps you synchronize consent states to Shopify, ensuring that tracking behavior aligns with user preferences for analytics, marketing, and personalization.

## How to use the Shopify Customer Privacy API Tag

1.  Add the **Shopify Customer Privacy API Tag** from the GTM Template Gallery to your Web container.
2.  Create a new tag and select "Shopify Customer Privacy API".
3.  Configure the tag settings based on your consent management setup.

### Consent Settings

You can set the consent source in two ways:

*   **Google Consent Mode**: Maps the consent status from Google's consent types (e.g., `analytics_storage`, `ad_storage`) to Shopify's consent properties (`analytics`, `marketing`, `preferences`).
*   **Manual**: Manually define the consent status for each Shopify consent property as `"granted"`, `"true"` or `true`. Everything else will be considered `"denied"`.

### Metafields

You can save custom data to the Shopify Customer Privacy API using [metafields](https://shopify.dev/docs/api/customer-privacy#metafields).

### Custom Storefront (Headless) Settings

If you are using a [custom storefront (headless commerce)](https://shopify.dev/docs/api/customer-privacy#metafields), you must provide the following details to ensure the API functions correctly:

* **Checkout Root Domain**: The domain of your checkout page (e.g., `checkout.example.com`).
* **Storefront Root Domain**: The domain of your custom storefront (e.g., `example.com`).
* **Storefront API Access Token**: Your public Storefront API access token.

## Useful Resources
* [Shopify Customer Privacy API](https://shopify.dev/docs/api/customer-privacy)

## Open Source

Initial development was done by [Lars Friis](https://www.linkedin.com/in/lars-friis/).

The **Shopify Customer Privacy API Tag for GTM Web** is developed and maintained by the [Stape Team](https://stape.io/) under the Apache 2.0 license.