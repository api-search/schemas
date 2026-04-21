---
description: Represents an ApplePayPaymentRequest used to configure an Apple Pay payment session, specifying the merchant capabilities, supported networks, payment amount, and optional shipping and billing requirements.
layout: schema
name: Apple Pay Payment Request
properties_list:
- description: The two-letter ISO 3166-1 alpha-2 country code for the merchant's country of operation
  name: countryCode
  type: string
- description: The three-letter ISO 4217 currency code for the payment
  name: currencyCode
  type: string
- description: The payment networks the merchant supports
  name: supportedNetworks
  type: array
- description: The payment capabilities the merchant supports
  name: merchantCapabilities
  type: array
- description: The total amount for the payment, including the merchant name as the label
  name: total
  type: object
- description: A list of line items explaining the charges, such as subtotal, tax, discount, and shipping
  name: lineItems
  type: array
- description: The billing contact fields required to process the payment
  name: requiredBillingContactFields
  type: array
- description: The shipping contact fields required to fulfill the order
  name: requiredShippingContactFields
  type: array
- description: Available shipping methods for the order
  name: shippingMethods
  type: array
- description: The type of shipping used for this request, which determines the wording on the payment sheet
  name: shippingType
  type: string
- description: Controls whether the shipping contact can be edited on the payment sheet
  name: shippingContactEditingMode
  type: string
- description: Base64-encoded application-specific data that is included in the payment token hash for verification
  name: applicationData
  type: string
- description: A list of ISO 3166-1 alpha-2 country codes for cards that can be used for payment. If not specified, all countries are supported
  name: supportedCountries
  type: array
- description: ''
  name: recurringPaymentRequest
  type: object
- description: ''
  name: automaticReloadPaymentRequest
  type: object
- description: An array of payment token contexts for multi-merchant payments
  name: multiTokenContexts
  type: array
provider_name: Apple Pay
provider_slug: apple-pay
schema_file: json-schema/apple-pay-payment-request-schema.json
slug: apple-pay-payment-request
tags:
- Apple
- Contactless Payments
- Digital Wallet
- E-Commerce
- Mobile Payments
- Payments
title: Apple Pay Payment Request
---
