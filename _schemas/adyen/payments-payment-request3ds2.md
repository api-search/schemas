---
description: PaymentRequest3ds2 schema from Adyen API
layout: schema
name: PaymentRequest3ds2
properties_list:
- description: Shopper account information for 3D Secure 2. > For 3D Secure 2 transactions, we recommend that you include this object to increase the chances of achieving a frictionless flow.
  name: accountInfo
  type: object
- description: If you want a [BIN or card verification](https://docs.adyen.com/payment-methods/cards/bin-data-and-card-verification) request to use a non-zero value, assign this value to `additionalAmount` (while th
  name: additionalAmount
  type: object
- description: This field contains additional data, which may be required for a particular payment request. The `additionalData` object consists of entries, each of which includes the key and value.
  name: additionalData
  type: object
- description: The amount information for the transaction (in [minor units](https://docs.adyen.com/development-resources/currency-codes)). For [BIN or card verification](https://docs.adyen.com/payment-methods/cards/
  name: amount
  type: object
- description: Information about your application. For more details, see [Building Adyen solutions](https://docs.adyen.com/development-resources/building-adyen-solutions).
  name: applicationInfo
  type: object
- description: The address where to send the invoice. > The `billingAddress` object is required in the following scenarios. Include all of the fields within this object. >* For 3D Secure 2 transactions in all browse
  name: billingAddress
  type: object
- description: The shopper's browser information. > For 3D Secure, the full object is required for web integrations. For mobile app integrations, include the `userAgent` and `acceptHeader` fields to indicate that yo
  name: browserInfo
  type: object
- description: The delay between the authorisation and scheduled auto-capture, specified in hours.
  name: captureDelayHours
  type: integer
- description: 'The shopper''s date of birth. Format [ISO-8601](https://www.w3.org/TR/NOTE-datetime): YYYY-MM-DD'
  name: dateOfBirth
  type: string
- description: The forex quote as returned in the response of the forex service.
  name: dccQuote
  type: object
- description: The address where the purchased goods should be delivered.
  name: deliveryAddress
  type: object
- description: 'The date and time the purchased goods should be delivered. Format [ISO 8601](https://www.w3.org/TR/NOTE-datetime): YYYY-MM-DDThh:mm:ss.sssTZD Example: 2017-07-17T13:42:40.428+01:00'
  name: deliveryDate
  type: string
- description: A string containing the shopper's device fingerprint. For more information, refer to [Device fingerprinting](https://docs.adyen.com/risk-management/device-fingerprinting).
  name: deviceFingerprint
  type: string
- description: An integer value that is added to the normal fraud score. The value can be either positive or negative.
  name: fraudOffset
  type: integer
- description: Contains installment settings. For more information, refer to [Installments](https://docs.adyen.com/payment-methods/cards/credit-card-installments).
  name: installments
  type: object
- description: The `localizedShopperStatement` field lets you use dynamic values for your shopper statement in a local character set. If not supplied, left empty, or for cross-border transactions, **shopperStatement
  name: localizedShopperStatement
  type: object
- description: The [merchant category code](https://en.wikipedia.org/wiki/Merchant_category_code) (MCC) is a four-digit number, which relates to a particular market segment. This code reflects the predominant activi
  name: mcc
  type: string
- description: The merchant account identifier, with which you want to process the transaction.
  name: merchantAccount
  type: string
- description: This reference allows linking multiple transactions to each other for reporting purposes (i.e. order auth-rate). The reference should be unique per billing cycle. The same merchant order reference sho
  name: merchantOrderReference
  type: string
- description: Additional risk fields for 3D Secure 2. > For 3D Secure 2 transactions, we recommend that you include this object to increase the chances of achieving a frictionless flow.
  name: merchantRiskIndicator
  type: object
- description: 'Metadata consists of entries, each of which includes a key and a value. Limits: * Maximum 20 key-value pairs per request. When exceeding, the "177" error occurs: "Metadata size exceeds limit". * Maxim'
  name: metadata
  type: object
- description: When you are doing multiple partial (gift card) payments, this is the `pspReference` of the first payment. We use this to link the multiple payments to each other. As your own reference for linking mu
  name: orderReference
  type: string
- description: The recurring settings for the payment. Use this property when you want to enable [recurring payments](https://docs.adyen.com/classic-integration/recurring-payments).
  name: recurring
  type: object
- description: 'Defines a recurring payment type. Required when creating a token to store payment details or using stored payment details. Allowed values: * `Subscription` – A transaction for a fixed or variable amou'
  name: recurringProcessingModel
  type: string
- description: The reference to uniquely identify a payment. This reference is used in all communication with you about the payment status. We recommend using a unique value per payment; however, it is not a require
  name: reference
  type: string
- description: 'Some payment methods require defining a value for this field to specify how to process the transaction. For the Bancontact payment method, it can be set to: * `maestro` (default), to be processed like'
  name: selectedBrand
  type: string
- description: The `recurringDetailReference` you want to use for this payment. The value `LATEST` can be used to select the most recently stored recurring detail.
  name: selectedRecurringDetailReference
  type: string
- description: A session ID used to identify a payment session.
  name: sessionId
  type: string
- description: The shopper's email address. We recommend that you provide this data, as it is used in velocity fraud checks. > For 3D Secure 2 transactions, schemes require `shopperEmail` for all browser-based and m
  name: shopperEmail
  type: string
- description: The shopper's IP address. In general, we recommend that you provide this data, as it is used in a number of risk checks (for instance, number of payment attempts or location-based checks). > For 3D Se
  name: shopperIP
  type: string
- description: Specifies the sales channel, through which the shopper gives their card details, and whether the shopper is a returning customer. For the web service API, Adyen assumes Ecommerce shopper interaction b
  name: shopperInteraction
  type: string
- description: The combination of a language code and a country code to specify the language to be used in the payment.
  name: shopperLocale
  type: string
- description: The shopper's full name.
  name: shopperName
  type: object
- description: 'Required for recurring payments. Your reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters. > Your reference must not include personally identif'
  name: shopperReference
  type: string
- description: 'The text to be shown on the shopper''s bank statement. We recommend sending a maximum of 22 characters, otherwise banks might truncate the string. Allowed characters: **a-z**, **A-Z**, **0-9**, spaces,'
  name: shopperStatement
  type: string
- description: The shopper's social security number.
  name: socialSecurityNumber
  type: string
- description: An array of objects specifying how the payment should be split when using [Adyen for Platforms](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#providing-split-information) or [I
  name: splits
  type: array
- description: 'The ecommerce or point-of-sale store that is processing the payment. Used in: * [Partner platform integrations](https://docs.adyen.com/marketplaces-and-platforms/classic/platforms-for-partners#route-p'
  name: store
  type: string
- description: The shopper's telephone number.
  name: telephoneNumber
  type: string
- description: Request fields for 3D Secure 2. To check if any of the following fields are required for your integration, refer to [Online payments](https://docs.adyen.com/online-payments) or [Classic integration](h
  name: threeDS2RequestData
  type: object
- description: Thre ThreeDS2Result that was returned in the final CRes.
  name: threeDS2Result
  type: object
- description: The ThreeDS2Token that was returned in the /authorise call.
  name: threeDS2Token
  type: string
- description: If set to true, you will only perform the [3D Secure 2 authentication](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only), and not the payment authorisation.
  name: threeDSAuthenticationOnly
  type: boolean
- description: The reference value to aggregate sales totals in reporting. When not specified, the store field is used (if available).
  name: totalsGroup
  type: string
- description: Set to true if the payment should be routed to a trusted MID.
  name: trustedShopper
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-payment-request3ds2-schema.json
slug: payments-payment-request3ds2
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-payment-request3ds2-schema.json\",\n  \"title\": \"PaymentRequest3ds2\",\n  \"description\": \"PaymentRequest3ds2 schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountInfo\": {\n      \"x-addedInVersion\": \"40\",\n      \"description\": \"Shopper account information for 3D Secure 2.\\n> For 3D Secure 2 transactions, we recommend that you include this object to increase the chances of achieving a frictionless flow.\",\n      \"$ref\": \"#/components/schemas/AccountInfo\"\n    },\n    \"additionalAmount\": {\n      \"description\": \"If you want a [BIN or card verification](https://docs.adyen.com/payment-methods/cards/bin-data-and-card-verification) request to use a non-zero value, assign this value to `additionalAmount` (while the amount must be still set to 0 to trigger\
  \ BIN or card verification).\\nRequired to be in the same currency as the `amount`. \",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"x-anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdditionalData3DSecure\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataAirline\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataCarRental\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataCommon\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataLevel23\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataLodging\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataOpenInvoice\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataOpi\"\n        },\n\
  \        {\n          \"$ref\": \"#/components/schemas/AdditionalDataRatepay\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataRetry\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataRisk\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataRiskStandalone\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataSubMerchant\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataTemporaryServices\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataWallets\"\n        }\n      ],\n      \"description\": \"This field contains additional data, which may be required for a particular payment request.\\n\\nThe `additionalData` object consists of entries, each of which includes the key and value.\",\n      \"type\": \"object\"\n    },\n    \"amount\": {\n      \"description\": \"The amount information for the transaction\
  \ (in [minor units](https://docs.adyen.com/development-resources/currency-codes)). For [BIN or card verification](https://docs.adyen.com/payment-methods/cards/bin-data-and-card-verification) requests, set amount to 0 (zero).\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"applicationInfo\": {\n      \"x-addedInVersion\": \"40\",\n      \"description\": \"Information about your application. For more details, see [Building Adyen solutions](https://docs.adyen.com/development-resources/building-adyen-solutions).\",\n      \"$ref\": \"#/components/schemas/ApplicationInfo\"\n    },\n    \"billingAddress\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The address where to send the invoice.\\n> The `billingAddress` object is required in the following scenarios. Include all of the fields within this object.\\n>* For 3D Secure 2 transactions in all browser-based and mobile implementations.\\n>* For cross-border payouts to and from Canada.\",\n      \"$ref\"\
  : \"#/components/schemas/Address\"\n    },\n    \"browserInfo\": {\n      \"description\": \"The shopper's browser information.\\n> For 3D Secure, the full object is required for web integrations. For mobile app integrations, include the `userAgent` and `acceptHeader` fields to indicate  that your integration can support a redirect in case a payment is routed to 3D Secure 1.\",\n      \"$ref\": \"#/components/schemas/BrowserInfo\"\n    },\n    \"captureDelayHours\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The delay between the authorisation and scheduled auto-capture, specified in hours.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"dateOfBirth\": {\n      \"x-addedInVersion\": \"7\",\n      \"description\": \"The shopper's date of birth.\\n\\nFormat [ISO-8601](https://www.w3.org/TR/NOTE-datetime): YYYY-MM-DD\",\n      \"format\": \"date\",\n      \"type\": \"string\"\n    },\n    \"dccQuote\": {\n      \"description\": \"The forex\
  \ quote as returned in the response of the forex service.\",\n      \"$ref\": \"#/components/schemas/ForexQuote\"\n    },\n    \"deliveryAddress\": {\n      \"description\": \"The address where the purchased goods should be delivered.\",\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"deliveryDate\": {\n      \"x-addedInVersion\": \"8\",\n      \"description\": \"The date and time the purchased goods should be delivered.\\n\\nFormat [ISO 8601](https://www.w3.org/TR/NOTE-datetime): YYYY-MM-DDThh:mm:ss.sssTZD\\n\\nExample: 2017-07-17T13:42:40.428+01:00\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"deviceFingerprint\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"A string containing the shopper's device fingerprint. For more information, refer to [Device fingerprinting](https://docs.adyen.com/risk-management/device-fingerprinting).\",\n      \"maxLength\": 5000,\n      \"type\": \"string\"\n    },\n    \"fraudOffset\":\
  \ {\n      \"description\": \"An integer value that is added to the normal fraud score. The value can be either positive or negative.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"installments\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"Contains installment settings. For more information, refer to [Installments](https://docs.adyen.com/payment-methods/cards/credit-card-installments).\",\n      \"$ref\": \"#/components/schemas/Installments\"\n    },\n    \"localizedShopperStatement\": {\n      \"x-addedInVersion\": \"68\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The `localizedShopperStatement` field lets you use dynamic values for your shopper statement in a local character set.\\nIf not supplied, left empty, or for cross-border transactions, **shopperStatement** is used.\\n\\nAdyen currently supports the ja-Kana character set for Visa and Mastercard payments in Japan using\
  \ Japanese cards. This character set supports:\\n\\n* UTF-8 based Katakana, capital letters, numbers and special characters. \\n* Half-width or full-width characters.\",\n      \"type\": \"object\"\n    },\n    \"mcc\": {\n      \"x-addedInVersion\": \"12\",\n      \"description\": \"The [merchant category code](https://en.wikipedia.org/wiki/Merchant_category_code) (MCC) is a four-digit number, which relates to a particular market segment. This code reflects the predominant activity that is conducted by the merchant.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier, with which you want to process the transaction.\",\n      \"type\": \"string\"\n    },\n    \"merchantOrderReference\": {\n      \"x-addedInVersion\": \"9\",\n      \"description\": \"This reference allows linking multiple transactions to each other for reporting purposes (i.e. order auth-rate). The reference should be unique per billing cycle.\\nThe\
  \ same merchant order reference should never be reused after the first authorised attempt. If used, this field should be supplied for all incoming authorisations.\\n> We strongly recommend you send the `merchantOrderReference` value to benefit from linking payment requests when authorisation retries take place. In addition, we recommend you provide `retry.orderAttemptNumber`, `retry.chainAttemptNumber`, and `retry.skipRetry` values in `PaymentRequest.additionalData`.\",\n      \"type\": \"string\"\n    },\n    \"merchantRiskIndicator\": {\n      \"x-addedInVersion\": \"40\",\n      \"description\": \"Additional risk fields for 3D Secure 2.\\n> For 3D Secure 2 transactions, we recommend that you include this object to increase the chances of achieving a frictionless flow.\",\n      \"$ref\": \"#/components/schemas/MerchantRiskIndicator\"\n    },\n    \"metadata\": {\n      \"x-addedInVersion\": \"17\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"\
  description\": \"Metadata consists of entries, each of which includes a key and a value.\\nLimits:\\n* Maximum 20 key-value pairs per request. When exceeding, the \\\"177\\\" error occurs: \\\"Metadata size exceeds limit\\\".\\n* Maximum 20 characters per key.\\n* Maximum 80 characters per value. \",\n      \"type\": \"object\"\n    },\n    \"orderReference\": {\n      \"description\": \"When you are doing multiple partial (gift card) payments, this is the `pspReference` of the first payment. We use this to link the multiple payments to each other. As your own reference for linking multiple payments, use the `merchantOrderReference`instead.\",\n      \"type\": \"string\"\n    },\n    \"recurring\": {\n      \"description\": \"The recurring settings for the payment. Use this property when you want to enable [recurring payments](https://docs.adyen.com/classic-integration/recurring-payments).\",\n      \"$ref\": \"#/components/schemas/Recurring\"\n    },\n    \"recurringProcessingModel\"\
  : {\n      \"x-addedInVersion\": \"30\",\n      \"description\": \"Defines a recurring payment type. Required when creating a token to store payment details or using stored payment details.\\nAllowed values:\\n* `Subscription` \\u2013 A transaction for a fixed or variable amount, which follows a fixed schedule.\\n* `CardOnFile` \\u2013 With a card-on-file (CoF) transaction, card details are stored to enable one-click or omnichannel journeys, or simply to streamline the checkout process. Any subscription not following a fixed schedule is also considered a card-on-file transaction.\\n* `UnscheduledCardOnFile` \\u2013 An unscheduled card-on-file (UCoF) transaction is a transaction that occurs on a non-fixed schedule and/or have variable amounts. For example, automatic top-ups when a cardholder's balance drops below a certain amount.\\n\",\n      \"enum\": [\n        \"CardOnFile\",\n        \"Subscription\",\n        \"UnscheduledCardOnFile\"\n      ],\n      \"type\": \"string\"\n    },\n\
  \    \"reference\": {\n      \"description\": \"The reference to uniquely identify a payment. This reference is used in all communication with you about the payment status. We recommend using a unique value per payment; however, it is not a requirement.\\nIf you need to provide multiple references for a transaction, separate them with hyphens (\\\"-\\\").\\nMaximum length: 80 characters.\",\n      \"type\": \"string\"\n    },\n    \"selectedBrand\": {\n      \"description\": \"Some payment methods require defining a value for this field to specify how to process the transaction.\\n\\nFor the Bancontact payment method, it can be set to:\\n* `maestro` (default), to be processed like a Maestro card, or\\n* `bcmc`, to be processed like a Bancontact card.\",\n      \"type\": \"string\"\n    },\n    \"selectedRecurringDetailReference\": {\n      \"description\": \"The `recurringDetailReference` you want to use for this payment. The value `LATEST` can be used to select the most recently stored\
  \ recurring detail.\",\n      \"type\": \"string\"\n    },\n    \"sessionId\": {\n      \"description\": \"A session ID used to identify a payment session.\",\n      \"type\": \"string\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"The shopper's email address. We recommend that you provide this data, as it is used in velocity fraud checks.\\n> For 3D Secure 2 transactions, schemes require `shopperEmail` for all browser-based and mobile implementations.\",\n      \"type\": \"string\"\n    },\n    \"shopperIP\": {\n      \"description\": \"The shopper's IP address. In general, we recommend that you provide this data, as it is used in a number of risk checks (for instance, number of payment attempts or location-based checks).\\n> For 3D Secure 2 transactions, schemes require `shopperIP` for all browser-based implementations.\\nThis field is also mandatory for some merchants depending on your business model. For more information, [contact Support](https://www.adyen.help/hc/en-us/requests/new).\"\
  ,\n      \"type\": \"string\"\n    },\n    \"shopperInteraction\": {\n      \"description\": \"Specifies the sales channel, through which the shopper gives their card details, and whether the shopper is a returning customer.\\nFor the web service API, Adyen assumes Ecommerce shopper interaction by default.\\n\\nThis field has the following possible values:\\n* `Ecommerce` - Online transactions where the cardholder is present (online). For better authorisation rates, we recommend sending the card security code (CSC) along with the request.\\n* `ContAuth` - Card on file and/or subscription transactions, where the cardholder is known to the merchant (returning customer). If the shopper is present (online), you can supply also the CSC to improve authorisation (one-click payment).\\n* `Moto` - Mail-order and telephone-order transactions where the shopper is in contact with the merchant via email or telephone.\\n* `POS` - Point-of-sale transactions where the shopper is physically present to\
  \ make a payment using a secure payment terminal.\",\n      \"enum\": [\n        \"Ecommerce\",\n        \"ContAuth\",\n        \"Moto\",\n        \"POS\"\n      ],\n      \"type\": \"string\"\n    },\n    \"shopperLocale\": {\n      \"x-addedInVersion\": \"7\",\n      \"description\": \"The combination of a language code and a country code to specify the language to be used in the payment.\",\n      \"type\": \"string\"\n    },\n    \"shopperName\": {\n      \"x-addedInVersion\": \"7\",\n      \"description\": \"The shopper's full name.\",\n      \"$ref\": \"#/components/schemas/Name\"\n    },\n    \"shopperReference\": {\n      \"description\": \"Required for recurring payments. \\nYour reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters.\\n> Your reference must not include personally identifiable information (PII), for example name or email address.\",\n      \"type\": \"string\"\n    },\n    \"shopperStatement\": {\n      \"\
  description\": \"The text to be shown on the shopper's bank statement.\\n We recommend sending a maximum of 22 characters, otherwise banks might truncate the string.\\n Allowed characters: **a-z**, **A-Z**, **0-9**, spaces, and special characters **. , ' _ - ? + * /**.\",\n      \"type\": \"string\"\n    },\n    \"socialSecurityNumber\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The shopper's social security number.\",\n      \"type\": \"string\"\n    },\n    \"splits\": {\n      \"x-addedInVersion\": \"37\",\n      \"description\": \"An array of objects specifying how the payment should be split when using [Adyen for Platforms](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#providing-split-information) or [Issuing](https://docs.adyen.com/issuing/add-manage-funds#split).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Split\"\n      },\n      \"type\": \"array\"\n    },\n    \"store\": {\n      \"x-addedInVersion\": \"23\",\n\
  \      \"description\": \"The ecommerce or point-of-sale store that is processing the payment. Used in:\\n\\n* [Partner platform integrations](https://docs.adyen.com/marketplaces-and-platforms/classic/platforms-for-partners#route-payments) for the [Classic Platforms integration](https://docs.adyen.com/marketplaces-and-platforms/classic).\\n* [Platform setup integrations](https://docs.adyen.com/marketplaces-and-platforms/additional-for-platform-setup/route-payment-to-store) for the [Balance Platform](https://docs.adyen.com/marketplaces-and-platforms).\",\n      \"maxLength\": 16,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    },\n    \"telephoneNumber\": {\n      \"x-addedInVersion\": \"7\",\n      \"description\": \"The shopper's telephone number.\",\n      \"type\": \"string\"\n    },\n    \"threeDS2RequestData\": {\n      \"x-addedInVersion\": \"40\",\n      \"description\": \"Request fields for 3D Secure 2. To check if any of the following fields are required for your integration,\
  \ refer to [Online payments](https://docs.adyen.com/online-payments) or [Classic integration](https://docs.adyen.com/classic-integration) documentation.\",\n      \"$ref\": \"#/components/schemas/ThreeDS2RequestData\"\n    },\n    \"threeDS2Result\": {\n      \"description\": \"Thre ThreeDS2Result that was returned in the final CRes.\",\n      \"$ref\": \"#/components/schemas/ThreeDS2Result\"\n    },\n    \"threeDS2Token\": {\n      \"description\": \"The ThreeDS2Token that was returned in the /authorise call.\",\n      \"type\": \"string\"\n    },\n    \"threeDSAuthenticationOnly\": {\n      \"x-addedInVersion\": \"50\",\n      \"default\": false,\n      \"description\": \"If set to true, you will only perform the [3D Secure 2 authentication](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only), and not the payment authorisation.\",\n      \"type\": \"boolean\"\n    },\n    \"totalsGroup\": {\n      \"x-addedInVersion\": \"23\",\n      \"description\"\
  : \"The reference value to aggregate sales totals in reporting. When not specified, the store field is used (if available).\",\n      \"maxLength\": 16,\n      \"minLength\": 1,\n      \"type\": \"string\"\n    },\n    \"trustedShopper\": {\n      \"x-addedInVersion\": \"37\",\n      \"description\": \"Set to true if the payment should be routed to a trusted MID.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n    \"reference\",\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-payment-request3ds2-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentRequest3ds2
---
