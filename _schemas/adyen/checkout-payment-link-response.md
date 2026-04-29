---
description: PaymentLinkResponse schema from Adyen API
layout: schema
name: PaymentLinkResponse
properties_list:
- description: 'List of payment methods to be presented to the shopper. To refer to payment methods, use their [payment method type](https://docs.adyen.com/payment-methods/payment-method-types). Example: `"allowedPay'
  name: allowedPaymentMethods
  type: array
- description: The payment amount and currency.
  name: amount
  type: object
- description: Information about your application. For more details, see [Building Adyen solutions](https://docs.adyen.com/development-resources/building-adyen-solutions).
  name: applicationInfo
  type: object
- description: The address where to send the invoice.
  name: billingAddress
  type: object
- description: 'List of payment methods to be hidden from the shopper. To refer to payment methods, use their [payment method type](https://docs.adyen.com/payment-methods/payment-method-types). Example: `"blockedPaym'
  name: blockedPaymentMethods
  type: array
- description: The delay between the authorisation and scheduled auto-capture, specified in hours.
  name: captureDelayHours
  type: integer
- description: The shopper's two-letter country code.
  name: countryCode
  type: string
- description: 'The shopper''s date of birth. Format [ISO-8601](https://www.w3.org/TR/NOTE-datetime): YYYY-MM-DD'
  name: dateOfBirth
  type: string
- description: 'The date and time when the purchased goods should be delivered. [ISO 8601](https://www.w3.org/TR/NOTE-datetime) format: YYYY-MM-DDThh:mm:ss+TZD, for example, **2020-12-18T10:15:30+01:00**.'
  name: deliverAt
  type: string
- description: The address where the purchased goods should be delivered.
  name: deliveryAddress
  type: object
- description: 'A short description visible on the payment page. Maximum length: 280 characters.'
  name: description
  type: string
- description: 'The date when the payment link expires. [ISO 8601](https://www.w3.org/TR/NOTE-datetime) format with time zone offset: YYYY-MM-DDThh:mm:ss+TZD, for example, **2020-12-18T10:15:30+01:00**. The maximum e'
  name: expiresAt
  type: string
- description: A unique identifier of the payment link.
  name: id
  type: string
- description: A set of key-value pairs that specifies the installment options available per payment method. The key must be a payment method name in lowercase. For example, **card** to specify installment options f
  name: installmentOptions
  type: object
- description: Price and product information about the purchased items, to be included on the invoice sent to the shopper. This parameter is required for open invoice (_buy now, pay later_) payment methods such Afte
  name: lineItems
  type: array
- description: Indicates if the payment must be [captured manually](https://docs.adyen.com/online-payments/capture).
  name: manualCapture
  type: boolean
- description: The [merchant category code](https://en.wikipedia.org/wiki/Merchant_category_code) (MCC) is a four-digit number, which relates to a particular market segment. This code reflects the predominant activi
  name: mcc
  type: string
- description: The merchant account identifier for which the payment link is created.
  name: merchantAccount
  type: string
- description: This reference allows linking multiple transactions to each other for reporting purposes (for example, order auth-rate). The reference should be unique per billing cycle.
  name: merchantOrderReference
  type: string
- description: 'Metadata consists of entries, each of which includes a key and a value. Limitations: * Maximum 20 key-value pairs per request. Otherwise, error "177" occurs: "Metadata size exceeds limit" * Maximum 20'
  name: metadata
  type: object
- description: 'Defines a recurring payment type. Required when `storePaymentMethodMode` is set to **askForConsent** or **enabled**. Possible values: * **Subscription** – A transaction for a fixed or variable amount,'
  name: recurringProcessingModel
  type: string
- description: A reference that is used to uniquely identify the payment in future communications about the payment status.
  name: reference
  type: string
- description: List of fields that the shopper has to provide on the payment page before completing the payment. For more information, refer to [Provide shopper information](https://docs.adyen.com/unified-commerce/p
  name: requiredShopperFields
  type: array
- description: Website URL used for redirection after payment is completed. If provided, a **Continue** button will be shown on the payment page. If shoppers select the button, they are redirected to the specified U
  name: returnUrl
  type: string
- description: Indicates whether the payment link can be reused for multiple payments. If not provided, this defaults to **false** which means the link can be used for one successful payment only.
  name: reusable
  type: boolean
- description: Any risk-related settings to apply to the payment.
  name: riskData
  type: object
- description: The shopper's email address.
  name: shopperEmail
  type: string
- description: The language to be used in the payment page, specified by a combination of a language and country code. For example, `en-US`. For a list of shopper locales that Pay by Link supports, refer to [Languag
  name: shopperLocale
  type: string
- description: The shopper's full name. This object is required for some payment methods such as AfterPay, Klarna, or if you're enrolled in the PayPal Seller Protection program.
  name: shopperName
  type: object
- description: 'Your reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters. > Your reference must not include personally identifiable information (PII), for exam'
  name: shopperReference
  type: string
- description: 'The text to be shown on the shopper''s bank statement. We recommend sending a maximum of 22 characters, otherwise banks might truncate the string. Allowed characters: **a-z**, **A-Z**, **0-9**, spaces,'
  name: shopperStatement
  type: string
- description: Set to **false** to hide the button that lets the shopper remove a stored payment method.
  name: showRemovePaymentMethodButton
  type: boolean
- description: The shopper's social security number.
  name: socialSecurityNumber
  type: string
- description: Boolean value indicating whether the card payment method should be split into separate debit and credit options.
  name: splitCardFundingSources
  type: boolean
- description: An array of objects specifying how to split a payment when using [Adyen for Platforms](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#providing-split-information), [Classic Plat
  name: splits
  type: array
- description: 'Status of the payment link. Possible values: * **active**: The link can be used to make payments. * **expired**: The expiry date for the payment link has passed. Shoppers can no longer use the link to'
  name: status
  type: string
- description: The physical store, for which this payment is processed.
  name: store
  type: string
- description: 'Indicates if the details of the payment method will be stored for the shopper. Possible values: * **disabled** – No details will be stored (default). * **askForConsent** – If the `shopperReference` is'
  name: storePaymentMethodMode
  type: string
- description: The shopper's telephone number.
  name: telephoneNumber
  type: string
- description: A [theme](https://docs.adyen.com/unified-commerce/pay-by-link/payment-links/api#themes) to customize the appearance of the payment page. If not specified, the payment page is rendered according to the
  name: themeId
  type: string
- description: 'The date when the payment link status was updated. [ISO 8601](https://www.w3.org/TR/NOTE-datetime) format: YYYY-MM-DDThh:mm:ss+TZD, for example, **2020-12-18T10:15:30+01:00**.'
  name: updatedAt
  type: string
- description: The URL at which the shopper can complete the payment.
  name: url
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-link-response-schema.json
slug: checkout-payment-link-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-link-response-schema.json\",\n  \"title\": \"PaymentLinkResponse\",\n  \"description\": \"PaymentLinkResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowedPaymentMethods\": {\n      \"description\": \"List of payment methods to be presented to the shopper. To refer to payment methods, use their [payment method type](https://docs.adyen.com/payment-methods/payment-method-types).\\n\\nExample: `\\\"allowedPaymentMethods\\\":[\\\"ideal\\\",\\\"giropay\\\"]`\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"amount\": {\n      \"description\": \"The payment amount and currency.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"applicationInfo\": {\n      \"description\": \"Information about\
  \ your application. For more details, see [Building Adyen solutions](https://docs.adyen.com/development-resources/building-adyen-solutions).\",\n      \"$ref\": \"#/components/schemas/ApplicationInfo\"\n    },\n    \"billingAddress\": {\n      \"description\": \"The address where to send the invoice.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"blockedPaymentMethods\": {\n      \"description\": \"List of payment methods to be hidden from the shopper. To refer to payment methods, use their [payment method type](https://docs.adyen.com/payment-methods/payment-method-types).\\n\\nExample: `\\\"blockedPaymentMethods\\\":[\\\"ideal\\\",\\\"giropay\\\"]`\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"captureDelayHours\": {\n      \"x-addedInVersion\": \"69\",\n      \"description\": \"The delay between the authorisation and scheduled auto-capture, specified in hours.\",\n      \"format\": \"int32\",\n      \"type\"\
  : \"integer\"\n    },\n    \"countryCode\": {\n      \"description\": \"The shopper's two-letter country code.\",\n      \"type\": \"string\"\n    },\n    \"dateOfBirth\": {\n      \"x-addedInVersion\": \"69\",\n      \"description\": \"The shopper's date of birth.\\n\\nFormat [ISO-8601](https://www.w3.org/TR/NOTE-datetime): YYYY-MM-DD\",\n      \"format\": \"date\",\n      \"type\": \"string\"\n    },\n    \"deliverAt\": {\n      \"description\": \"The date and time when the purchased goods should be delivered.\\n\\n[ISO 8601](https://www.w3.org/TR/NOTE-datetime) format: YYYY-MM-DDThh:mm:ss+TZD, for example, **2020-12-18T10:15:30+01:00**.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"deliveryAddress\": {\n      \"description\": \"The address where the purchased goods should be delivered.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"description\": {\n      \"description\": \"A short description visible on the payment page.\\nMaximum\
  \ length: 280 characters.\",\n      \"type\": \"string\"\n    },\n    \"expiresAt\": {\n      \"x-addedInVersion\": \"71\",\n      \"description\": \"The date when the payment link expires.\\n\\n[ISO 8601](https://www.w3.org/TR/NOTE-datetime) format with time zone offset: YYYY-MM-DDThh:mm:ss+TZD, for example, **2020-12-18T10:15:30+01:00**.\\n\\nThe maximum expiry date is 70 days after the payment link is created.\\n\\nIf not provided, the payment link expires 24 hours after it was created.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"x-addedInVersion\": \"51\",\n      \"description\": \"A unique identifier of the payment link.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"installmentOptions\": {\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/InstallmentOption\"\n      },\n      \"description\": \"A set of key-value pairs that specifies the installment options available per payment\
  \ method. The key must be a payment method name in lowercase. For example, **card** to specify installment options for all cards, or **visa** or **mc**. The value must be an object containing the installment options.\",\n      \"type\": \"object\"\n    },\n    \"lineItems\": {\n      \"description\": \"Price and product information about the purchased items, to be included on the invoice sent to the shopper.\\nThis parameter is required for open invoice (_buy now, pay later_) payment methods such Afterpay, Clearpay, Klarna, RatePay, and Zip.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LineItem\"\n      },\n      \"type\": \"array\"\n    },\n    \"manualCapture\": {\n      \"description\": \"Indicates if the payment must be [captured manually](https://docs.adyen.com/online-payments/capture).\",\n      \"type\": \"boolean\"\n    },\n    \"mcc\": {\n      \"x-addedInVersion\": \"69\",\n      \"description\": \"The [merchant category code](https://en.wikipedia.org/wiki/Merchant_category_code)\
  \ (MCC) is a four-digit number, which relates to a particular market segment. This code reflects the predominant activity that is conducted by the merchant.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier for which the payment link is created.\",\n      \"type\": \"string\"\n    },\n    \"merchantOrderReference\": {\n      \"description\": \"This reference allows linking multiple transactions to each other for reporting purposes (for example, order auth-rate). The reference should be unique per billing cycle.\",\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Metadata consists of entries, each of which includes a key and a value.\\nLimitations:\\n* Maximum 20 key-value pairs per request. Otherwise, error \\\"177\\\" occurs: \\\"Metadata size exceeds limit\\\"\\n* Maximum 20 characters per key. Otherwise,\
  \ error \\\"178\\\" occurs: \\\"Metadata key size exceeds limit\\\"\\n* A key cannot have the name `checkout.linkId`. Any value that you provide with this key is going to be replaced by the real payment link ID.\",\n      \"maxLength\": 80,\n      \"type\": \"object\"\n    },\n    \"recurringProcessingModel\": {\n      \"description\": \"Defines a recurring payment type. Required when `storePaymentMethodMode` is set to **askForConsent** or **enabled**.\\nPossible values:\\n* **Subscription** \\u2013 A transaction for a fixed or variable amount, which follows a fixed schedule.\\n* **CardOnFile** \\u2013 With a card-on-file (CoF) transaction, card details are stored to enable one-click or omnichannel journeys, or simply to streamline the checkout process. Any subscription not following a fixed schedule is also considered a card-on-file transaction.\\n* **UnscheduledCardOnFile** \\u2013 An unscheduled card-on-file (UCoF) transaction is a transaction that occurs on a non-fixed schedule and/or\
  \ has variable amounts. For example, automatic top-ups when a cardholder's balance drops below a certain amount.\\n\",\n      \"enum\": [\n        \"CardOnFile\",\n        \"Subscription\",\n        \"UnscheduledCardOnFile\"\n      ],\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"A reference that is used to uniquely identify the payment in future communications about the payment status.\",\n      \"type\": \"string\"\n    },\n    \"requiredShopperFields\": {\n      \"x-addedInVersion\": \"67\",\n      \"description\": \"List of fields that the shopper has to provide on the payment page before completing the payment. For more information, refer to [Provide shopper information](https://docs.adyen.com/unified-commerce/pay-by-link/payment-links/api#shopper-information).\\n\\nPossible values:\\n* **billingAddress** \\u2013 The address where to send the invoice.\\n* **deliveryAddress** \\u2013 The address where the purchased goods should be delivered.\\\
  n* **shopperEmail** \\u2013 The shopper's email address.\\n* **shopperName** \\u2013 The shopper's full name.\\n* **telephoneNumber** \\u2013 The shopper's phone number.\\n\",\n      \"items\": {\n        \"enum\": [\n          \"billingAddress\",\n          \"deliveryAddress\",\n          \"shopperEmail\",\n          \"shopperName\",\n          \"telephoneNumber\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"returnUrl\": {\n      \"description\": \"Website URL used for redirection after payment is completed.\\nIf provided, a **Continue** button will be shown on the payment page. If shoppers select the button, they are redirected to the specified URL.\",\n      \"type\": \"string\"\n    },\n    \"reusable\": {\n      \"description\": \"Indicates whether the payment link can be reused for multiple payments. If not provided, this defaults to **false** which means the link can be used for one successful payment only.\",\n      \"type\": \"\
  boolean\"\n    },\n    \"riskData\": {\n      \"x-addedInVersion\": \"65\",\n      \"description\": \"Any risk-related settings to apply to the payment.\",\n      \"$ref\": \"#/components/schemas/RiskData\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"The shopper's email address.\",\n      \"type\": \"string\"\n    },\n    \"shopperLocale\": {\n      \"description\": \"The language to be used in the payment page, specified by a combination of a language and country code. For example, `en-US`.\\n\\nFor a list of shopper locales that Pay by Link supports, refer to [Language and localization](https://docs.adyen.com/unified-commerce/pay-by-link/payment-links/api#language).\",\n      \"type\": \"string\"\n    },\n    \"shopperName\": {\n      \"description\": \"The shopper's full name. This object is required for some payment methods such as AfterPay, Klarna, or if you're enrolled in the PayPal Seller Protection program.\",\n      \"$ref\": \"#/components/schemas/Name\"\n    },\n\
  \    \"shopperReference\": {\n      \"description\": \"Your reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters.\\n> Your reference must not include personally identifiable information (PII), for example name or email address.\",\n      \"maxLength\": 256,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"shopperStatement\": {\n      \"x-addedInVersion\": \"69\",\n      \"description\": \"The text to be shown on the shopper's bank statement.\\n We recommend sending a maximum of 22 characters, otherwise banks might truncate the string.\\n Allowed characters: **a-z**, **A-Z**, **0-9**, spaces, and special characters **. , ' _ - ? + * /**.\",\n      \"type\": \"string\"\n    },\n    \"showRemovePaymentMethodButton\": {\n      \"default\": true,\n      \"description\": \"Set to **false** to hide the button that lets the shopper remove a stored payment method.\",\n      \"type\": \"boolean\"\n    },\n    \"socialSecurityNumber\"\
  : {\n      \"x-addedInVersion\": \"69\",\n      \"description\": \"The shopper's social security number.\",\n      \"type\": \"string\"\n    },\n    \"splitCardFundingSources\": {\n      \"x-addedInVersion\": \"69\",\n      \"default\": false,\n      \"description\": \"Boolean value indicating whether the card payment method should be split into separate debit and credit options.\",\n      \"type\": \"boolean\"\n    },\n    \"splits\": {\n      \"description\": \"An array of objects specifying how to split a payment when using [Adyen for Platforms](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#providing-split-information), [Classic Platforms integration](https://docs.adyen.com/marketplaces-and-platforms/classic/processing-payments#providing-split-information), or [Issuing](https://docs.adyen.com/issuing/manage-funds#split).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Split\"\n      },\n      \"type\": \"array\"\n    },\n    \"status\": {\n \
  \     \"description\": \"Status of the payment link. Possible values:\\n* **active**: The link can be used to make payments.\\n* **expired**: The expiry date for the payment link has passed. Shoppers can no longer use the link to make payments.\\n* **completed**: The shopper completed the payment.\\n* **paymentPending**: The shopper is in the process of making the payment. Applies to payment methods with an asynchronous flow.\",\n      \"enum\": [\n        \"active\",\n        \"completed\",\n        \"expired\",\n        \"paid\",\n        \"paymentPending\"\n      ],\n      \"type\": \"string\"\n    },\n    \"store\": {\n      \"description\": \"The physical store, for which this payment is processed.\",\n      \"type\": \"string\"\n    },\n    \"storePaymentMethodMode\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"Indicates if the details of the payment method will be stored for the shopper. Possible values:\\n* **disabled** \\u2013 No details will be stored (default).\\\
  n* **askForConsent** \\u2013 If the `shopperReference` is provided, the UI lets the shopper choose if they want their payment details to be stored.\\n* **enabled** \\u2013 If the `shopperReference` is provided, the details will be stored without asking the shopper for consent. \\n When set to **askForConsent** or **enabled**, you must also include the `recurringProcessingModel` parameter.\",\n      \"enum\": [\n        \"askForConsent\",\n        \"disabled\",\n        \"enabled\"\n      ],\n      \"type\": \"string\"\n    },\n    \"telephoneNumber\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The shopper's telephone number.\",\n      \"type\": \"string\"\n    },\n    \"themeId\": {\n      \"x-addedInVersion\": \"67\",\n      \"description\": \"A [theme](https://docs.adyen.com/unified-commerce/pay-by-link/payment-links/api#themes) to customize the appearance of the payment page. If not specified, the payment page is rendered according to the theme set as default in\
  \ your Customer Area.\",\n      \"type\": \"string\"\n    },\n    \"updatedAt\": {\n      \"description\": \"The date when the payment link status was updated.\\n\\n[ISO 8601](https://www.w3.org/TR/NOTE-datetime) format: YYYY-MM-DDThh:mm:ss+TZD, for example, **2020-12-18T10:15:30+01:00**.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"url\": {\n      \"description\": \"The URL at which the shopper can complete the payment.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"amount\",\n    \"reference\",\n    \"merchantAccount\",\n    \"id\",\n    \"url\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-link-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentLinkResponse
---
