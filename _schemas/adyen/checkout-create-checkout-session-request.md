---
description: CreateCheckoutSessionRequest schema from Adyen API
layout: schema
name: CreateCheckoutSessionRequest
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
- description: 'List of payment methods to be presented to the shopper. To refer to payment methods, use their [payment method type](https://docs.adyen.com/payment-methods/payment-method-types). Example: `"allowedPay'
  name: allowedPaymentMethods
  type: array
- description: The amount of the payment.
  name: amount
  type: object
- description: Information about your application. For more details, see [Building Adyen solutions](https://docs.adyen.com/development-resources/building-adyen-solutions).
  name: applicationInfo
  type: object
- description: Configuration data for 3DS payments.
  name: authenticationData
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
- description: The platform where a payment transaction takes place. This field is optional for filtering out payment methods that are only available on specific platforms. If this value is not set, then we will try
  name: channel
  type: string
- description: Information regarding the company.
  name: company
  type: object
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
- description: When true and `shopperReference` is provided, the shopper will be asked if the payment details should be stored for future one-click payments.
  name: enableOneClick
  type: boolean
- description: When true and `shopperReference` is provided, the payment details will be tokenized for payouts.
  name: enablePayOut
  type: boolean
- description: When true and `shopperReference` is provided, the payment details will be tokenized for recurring payments.
  name: enableRecurring
  type: boolean
- description: The date the session expires in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format. When not specified, the expiry date is set to 1 hour after session creation. You cannot set th
  name: expiresAt
  type: string
- description: The person or entity funding the money.
  name: fundOrigin
  type: object
- description: the person or entity receiving the money
  name: fundRecipient
  type: object
- description: A set of key-value pairs that specifies the installment options available per payment method. The key must be a payment method name in lowercase. For example, **card** to specify installment options f
  name: installmentOptions
  type: object
- description: Price and product information about the purchased items, to be included on the invoice sent to the shopper. > This field is required for 3x 4x Oney, Affirm, Afterpay, Clearpay, Klarna, Ratepay, and Zi
  name: lineItems
  type: array
- description: The mandate details to initiate recurring transaction.
  name: mandate
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
- description: 'Metadata consists of entries, each of which includes a key and a value. Limits: * Maximum 20 key-value pairs per request. * Maximum 20 characters per key. * Maximum 80 characters per value.'
  name: metadata
  type: object
- description: 'Indicates the type of front end integration. Possible values: * **embedded** (default): Drop-in or Components integration * **hosted**: Hosted Checkout integration'
  name: mode
  type: string
- description: Authentication data produced by an MPI (Mastercard SecureCode, Visa Secure, or Cartes Bancaires).
  name: mpiData
  type: object
- description: Defines how to book chargebacks when using [Adyen for Platforms](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#chargebacks-and-disputes).
  name: platformChargebackLogic
  type: object
- description: Date after which no further authorisations shall be performed. Only for 3D Secure 2.
  name: recurringExpiry
  type: string
- description: Minimum number of days between authorisations. Only for 3D Secure 2.
  name: recurringFrequency
  type: string
- description: 'Defines a recurring payment type. Required when creating a token to store payment details. Allowed values: * `Subscription` – A transaction for a fixed or variable amount, which follows a fixed schedu'
  name: recurringProcessingModel
  type: string
- description: Specifies the redirect method (GET or POST) when redirecting back from the issuer.
  name: redirectFromIssuerMethod
  type: string
- description: Specifies the redirect method (GET or POST) when redirecting to the issuer.
  name: redirectToIssuerMethod
  type: string
- description: The reference to uniquely identify a payment.
  name: reference
  type: string
- description: The URL to return to when a redirect payment is completed.
  name: returnUrl
  type: string
- description: Any risk-related settings to apply to the payment.
  name: riskData
  type: object
- description: The shopper's email address.
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
- description: The shopper's full name. This object is required for some payment methods such as AfterPay, Klarna, or if you're enrolled in the PayPal Seller Protection program.
  name: shopperName
  type: object
- description: 'Your reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters. > Your reference must not include personally identifiable information (PII), for exam'
  name: shopperReference
  type: string
- description: 'The text to be shown on the shopper''s bank statement. We recommend sending a maximum of 22 characters, otherwise banks might truncate the string. Allowed characters: **a-z**, **A-Z**, **0-9**, spaces,'
  name: shopperStatement
  type: string
- description: Set to true to show the payment amount per installment.
  name: showInstallmentAmount
  type: boolean
- description: Set to **true** to show a button that lets the shopper remove a stored payment method.
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
- description: Required for Adyen for Platforms integrations if you have a platform setup. This is your [reference](https://docs.adyen.com/api-explorer/Management/3/post/merchants/(merchantId)/stores#request-referen
  name: store
  type: string
- description: When this is set to **true** and the `shopperReference` is provided, the payment details will be stored.
  name: storePaymentMethod
  type: boolean
- description: 'Indicates if the details of the payment method will be stored for the shopper. Possible values: * **disabled** – No details will be stored (default). * **askForConsent** – If the `shopperReference` is'
  name: storePaymentMethodMode
  type: string
- description: The shopper's telephone number.
  name: telephoneNumber
  type: string
- description: Sets a custom theme for [Hosted Checkout](https://docs.adyen.com/online-payments/build-your-integration/?platform=Web&integration=Hosted+Checkout). The value can be any of the **Theme ID** values from
  name: themeId
  type: string
- description: If set to true, you will only perform the [3D Secure 2 authentication](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only), and not the payment authorisation.
  name: threeDSAuthenticationOnly
  type: boolean
- description: Set to true if the payment should be routed to a trusted MID.
  name: trustedShopper
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-create-checkout-session-request-schema.json
slug: checkout-create-checkout-session-request
source_filename: checkout-create-checkout-session-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-create-checkout-session-request-schema.json\",\n  \"title\": \"CreateCheckoutSessionRequest\",\n  \"description\": \"CreateCheckoutSessionRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountInfo\": {\n      \"description\": \"Shopper account information for 3D Secure 2.\\n> For 3D Secure 2 transactions, we recommend that you include this object to increase the chances of achieving a frictionless flow.\",\n      \"$ref\": \"#/components/schemas/AccountInfo\"\n    },\n    \"additionalAmount\": {\n      \"description\": \"If you want a [BIN or card verification](https://docs.adyen.com/payment-methods/cards/bin-data-and-card-verification) request to use a non-zero value, assign this value to `additionalAmount` (while the amount must be still set to 0 to trigger BIN or\
  \ card verification).\\nRequired to be in the same currency as the `amount`. \",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"x-anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdditionalData3DSecure\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataAirline\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataCarRental\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataCommon\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataLevel23\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataLodging\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataOpenInvoice\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataOpi\"\n        },\n      \
  \  {\n          \"$ref\": \"#/components/schemas/AdditionalDataRatepay\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataRetry\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataRisk\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataRiskStandalone\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataSubMerchant\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataTemporaryServices\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AdditionalDataWallets\"\n        }\n      ],\n      \"description\": \"This field contains additional data, which may be required for a particular payment request.\\n\\nThe `additionalData` object consists of entries, each of which includes the key and value.\",\n      \"type\": \"object\"\n    },\n    \"allowedPaymentMethods\": {\n      \"description\": \"List of payment methods to be\
  \ presented to the shopper. To refer to payment methods, use their [payment method type](https://docs.adyen.com/payment-methods/payment-method-types).\\n\\nExample: `\\\"allowedPaymentMethods\\\":[\\\"ideal\\\",\\\"giropay\\\"]`\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"amount\": {\n      \"description\": \"The amount of the payment.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"applicationInfo\": {\n      \"description\": \"Information about your application. For more details, see [Building Adyen solutions](https://docs.adyen.com/development-resources/building-adyen-solutions).\",\n      \"$ref\": \"#/components/schemas/ApplicationInfo\"\n    },\n    \"authenticationData\": {\n      \"x-addedInVersion\": \"69\",\n      \"description\": \"Configuration data for 3DS payments.\",\n      \"$ref\": \"#/components/schemas/AuthenticationData\"\n    },\n    \"billingAddress\": {\n      \"description\": \"The address\
  \ where to send the invoice.\",\n      \"$ref\": \"#/components/schemas/BillingAddress\"\n    },\n    \"blockedPaymentMethods\": {\n      \"description\": \"List of payment methods to be hidden from the shopper. To refer to payment methods, use their [payment method type](https://docs.adyen.com/payment-methods/payment-method-types).\\n\\nExample: `\\\"blockedPaymentMethods\\\":[\\\"ideal\\\",\\\"giropay\\\"]`\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"captureDelayHours\": {\n      \"description\": \"The delay between the authorisation and scheduled auto-capture, specified in hours.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"channel\": {\n      \"description\": \"The platform where a payment transaction takes place. This field is optional for filtering out payment methods that are only available on specific platforms. If this value is not set, then we will try to infer it from the `sdkVersion`\
  \ or `token`.\\n\\nPossible values:\\n* **iOS**\\n* **Android**\\n* **Web**\",\n      \"enum\": [\n        \"iOS\",\n        \"Android\",\n        \"Web\"\n      ],\n      \"type\": \"string\"\n    },\n    \"company\": {\n      \"description\": \"Information regarding the company.\",\n      \"$ref\": \"#/components/schemas/Company\"\n    },\n    \"countryCode\": {\n      \"description\": \"The shopper's two-letter country code.\",\n      \"type\": \"string\"\n    },\n    \"dateOfBirth\": {\n      \"description\": \"The shopper's date of birth.\\n\\nFormat [ISO-8601](https://www.w3.org/TR/NOTE-datetime): YYYY-MM-DD\",\n      \"format\": \"date\",\n      \"type\": \"string\"\n    },\n    \"deliverAt\": {\n      \"description\": \"The date and time when the purchased goods should be delivered.\\n\\n[ISO 8601](https://www.w3.org/TR/NOTE-datetime) format: YYYY-MM-DDThh:mm:ss+TZD, for example, **2020-12-18T10:15:30+01:00**.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n \
  \   },\n    \"deliveryAddress\": {\n      \"description\": \"The address where the purchased goods should be delivered.\",\n      \"$ref\": \"#/components/schemas/DeliveryAddress\"\n    },\n    \"enableOneClick\": {\n      \"description\": \"When true and `shopperReference` is provided, the shopper will be asked if the payment details should be stored for future one-click payments.\",\n      \"type\": \"boolean\"\n    },\n    \"enablePayOut\": {\n      \"description\": \"When true and `shopperReference` is provided, the payment details will be tokenized for payouts.\",\n      \"type\": \"boolean\"\n    },\n    \"enableRecurring\": {\n      \"description\": \"When true and `shopperReference` is provided, the payment details will be tokenized for recurring payments.\",\n      \"type\": \"boolean\"\n    },\n    \"expiresAt\": {\n      \"description\": \"The date the session expires in [ISO8601](https://www.iso.org/iso-8601-date-and-time-format.html) format. When not specified, the expiry\
  \ date is set to 1 hour after session creation. You cannot set the session expiry to more than 24 hours after session creation.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"fundOrigin\": {\n      \"description\": \"The person or entity funding the money.\",\n      \"$ref\": \"#/components/schemas/FundOrigin\"\n    },\n    \"fundRecipient\": {\n      \"description\": \"the person or entity receiving the money\",\n      \"$ref\": \"#/components/schemas/FundRecipient\"\n    },\n    \"installmentOptions\": {\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/CheckoutSessionInstallmentOption\"\n      },\n      \"description\": \"A set of key-value pairs that specifies the installment options available per payment method. The key must be a payment method name in lowercase. For example, **card** to specify installment options for all cards, or **visa** or **mc**. The value must be an object containing the installment options.\",\n \
  \     \"type\": \"object\"\n    },\n    \"lineItems\": {\n      \"description\": \"Price and product information about the purchased items, to be included on the invoice sent to the shopper.\\n> This field is required for 3x 4x Oney, Affirm, Afterpay, Clearpay, Klarna, Ratepay, and Zip.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LineItem\"\n      },\n      \"type\": \"array\"\n    },\n    \"mandate\": {\n      \"description\": \"The mandate details to initiate recurring transaction.\",\n      \"$ref\": \"#/components/schemas/Mandate\"\n    },\n    \"mcc\": {\n      \"description\": \"The [merchant category code](https://en.wikipedia.org/wiki/Merchant_category_code) (MCC) is a four-digit number, which relates to a particular market segment. This code reflects the predominant activity that is conducted by the merchant.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier, with which you want to\
  \ process the transaction.\",\n      \"type\": \"string\"\n    },\n    \"merchantOrderReference\": {\n      \"description\": \"This reference allows linking multiple transactions to each other for reporting purposes (i.e. order auth-rate). The reference should be unique per billing cycle.\\nThe same merchant order reference should never be reused after the first authorised attempt. If used, this field should be supplied for all incoming authorisations.\\n> We strongly recommend you send the `merchantOrderReference` value to benefit from linking payment requests when authorisation retries take place. In addition, we recommend you provide `retry.orderAttemptNumber`, `retry.chainAttemptNumber`, and `retry.skipRetry` values in `PaymentRequest.additionalData`.\",\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Metadata consists of entries, each of which includes a key and a value.\\\
  nLimits:\\n* Maximum 20 key-value pairs per request.\\n* Maximum 20 characters per key.\\n* Maximum 80 characters per value. \",\n      \"type\": \"object\"\n    },\n    \"mode\": {\n      \"x-addedInVersion\": \"69\",\n      \"default\": \"embedded\",\n      \"description\": \"Indicates the type of front end integration. Possible values:\\n* **embedded** (default): Drop-in or Components integration\\n* **hosted**: Hosted Checkout integration\",\n      \"enum\": [\n        \"embedded\",\n        \"hosted\"\n      ],\n      \"type\": \"string\"\n    },\n    \"mpiData\": {\n      \"description\": \"Authentication data produced by an MPI (Mastercard SecureCode, Visa Secure, or Cartes Bancaires).\",\n      \"$ref\": \"#/components/schemas/ThreeDSecureData\"\n    },\n    \"platformChargebackLogic\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"Defines how to book chargebacks when using [Adyen for Platforms](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#chargebacks-and-disputes).\"\
  ,\n      \"$ref\": \"#/components/schemas/PlatformChargebackLogic\"\n    },\n    \"recurringExpiry\": {\n      \"description\": \"Date after which no further authorisations shall be performed. Only for 3D Secure 2.\",\n      \"type\": \"string\"\n    },\n    \"recurringFrequency\": {\n      \"description\": \"Minimum number of days between authorisations. Only for 3D Secure 2.\",\n      \"type\": \"string\"\n    },\n    \"recurringProcessingModel\": {\n      \"description\": \"Defines a recurring payment type. Required when creating a token to store payment details.\\nAllowed values:\\n* `Subscription` \\u2013 A transaction for a fixed or variable amount, which follows a fixed schedule.\\n* `CardOnFile` \\u2013 With a card-on-file (CoF) transaction, card details are stored to enable one-click or omnichannel journeys, or simply to streamline the checkout process. Any subscription not following a fixed schedule is also considered a card-on-file transaction.\\n* `UnscheduledCardOnFile` \\\
  u2013 An unscheduled card-on-file (UCoF) transaction is a transaction that occurs on a non-fixed schedule and/or have variable amounts. For example, automatic top-ups when a cardholder's balance drops below a certain amount.\\n\",\n      \"enum\": [\n        \"CardOnFile\",\n        \"Subscription\",\n        \"UnscheduledCardOnFile\"\n      ],\n      \"type\": \"string\"\n    },\n    \"redirectFromIssuerMethod\": {\n      \"description\": \"Specifies the redirect method (GET or POST) when redirecting back from the issuer.\",\n      \"type\": \"string\"\n    },\n    \"redirectToIssuerMethod\": {\n      \"description\": \"Specifies the redirect method (GET or POST) when redirecting to the issuer.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"The reference to uniquely identify a payment.\",\n      \"type\": \"string\"\n    },\n    \"returnUrl\": {\n      \"description\": \"The URL to return to when a redirect payment is completed.\",\n      \"type\"\
  : \"string\"\n    },\n    \"riskData\": {\n      \"description\": \"Any risk-related settings to apply to the payment.\",\n      \"$ref\": \"#/components/schemas/RiskData\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"The shopper's email address.\",\n      \"type\": \"string\"\n    },\n    \"shopperIP\": {\n      \"description\": \"The shopper's IP address. In general, we recommend that you provide this data, as it is used in a number of risk checks (for instance, number of payment attempts or location-based checks).\\n> For 3D Secure 2 transactions, schemes require `shopperIP` for all browser-based implementations.\\nThis field is also mandatory for some merchants depending on your business model. For more information, [contact Support](https://www.adyen.help/hc/en-us/requests/new).\",\n      \"type\": \"string\"\n    },\n    \"shopperInteraction\": {\n      \"description\": \"Specifies the sales channel, through which the shopper gives their card details, and whether the\
  \ shopper is a returning customer.\\nFor the web service API, Adyen assumes Ecommerce shopper interaction by default.\\n\\nThis field has the following possible values:\\n* `Ecommerce` - Online transactions where the cardholder is present (online). For better authorisation rates, we recommend sending the card security code (CSC) along with the request.\\n* `ContAuth` - Card on file and/or subscription transactions, where the cardholder is known to the merchant (returning customer). If the shopper is present (online), you can supply also the CSC to improve authorisation (one-click payment).\\n* `Moto` - Mail-order and telephone-order transactions where the shopper is in contact with the merchant via email or telephone.\\n* `POS` - Point-of-sale transactions where the shopper is physically present to make a payment using a secure payment terminal.\",\n      \"enum\": [\n        \"Ecommerce\",\n        \"ContAuth\",\n        \"Moto\",\n        \"POS\"\n      ],\n      \"type\": \"string\"\
  \n    },\n    \"shopperLocale\": {\n      \"description\": \"The combination of a language code and a country code to specify the language to be used in the payment.\",\n      \"type\": \"string\"\n    },\n    \"shopperName\": {\n      \"description\": \"The shopper's full name. This object is required for some payment methods such as AfterPay, Klarna, or if you're enrolled in the PayPal Seller Protection program.\",\n      \"$ref\": \"#/components/schemas/Name\"\n    },\n    \"shopperReference\": {\n      \"description\": \"Your reference to uniquely identify this shopper, for example user ID or account ID. Minimum length: 3 characters.\\n> Your reference must not include personally identifiable information (PII), for example name or email address.\",\n      \"maxLength\": 256,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"shopperStatement\": {\n      \"description\": \"The text to be shown on the shopper's bank statement.\\n We recommend sending a maximum of 22\
  \ characters, otherwise banks might truncate the string.\\n Allowed characters: **a-z**, **A-Z**, **0-9**, spaces, and special characters **. , ' _ - ? + * /**.\",\n      \"type\": \"string\"\n    },\n    \"showInstallmentAmount\": {\n      \"description\": \"Set to true to show the payment amount per installment.\",\n      \"type\": \"boolean\"\n    },\n    \"showRemovePaymentMethodButton\": {\n      \"description\": \"Set to **true** to show a button that lets the shopper remove a stored payment method.\",\n      \"type\": \"boolean\"\n    },\n    \"socialSecurityNumber\": {\n      \"description\": \"The shopper's social security number.\",\n      \"type\": \"string\"\n    },\n    \"splitCardFundingSources\": {\n      \"default\": false,\n      \"description\": \"Boolean value indicating whether the card payment method should be split into separate debit and credit options.\",\n      \"type\": \"boolean\"\n    },\n    \"splits\": {\n      \"description\": \"An array of objects specifying\
  \ how to split a payment when using [Adyen for Platforms](https://docs.adyen.com/marketplaces-and-platforms/processing-payments#providing-split-information), [Classic Platforms integration](https://docs.adyen.com/marketplaces-and-platforms/classic/processing-payments#providing-split-information), or [Issuing](https://docs.adyen.com/issuing/manage-funds#split).\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Split\"\n      },\n      \"type\": \"array\"\n    },\n    \"store\": {\n      \"description\": \"Required for Adyen for Platforms integrations if you have a platform setup. This is your [reference](https://docs.adyen.com/api-explorer/Management/3/post/merchants/(merchantId)/stores#request-reference) (on [balance platform](https://docs.adyen.com/marketplaces-and-platforms/classic/platforms-for-partners#route-payments)) or the [storeReference](https://docs.adyen.com/api-explorer/Account/latest/post/updateAccountHolder#request-accountHolderDetails-storeDetails-storeReference)\
  \ (in the [classic integration](https://docs.adyen.com/marketplaces-and-platforms/processing-payments/route-payment-to-store/#route-a-payment-to-a-store)) for the ecommerce or point-of-sale store that is processing the payment.\",\n      \"type\": \"string\"\n    },\n    \"storePaymentMethod\": {\n      \"description\": \"When this is set to **true** and the `shopperReference` is provided, the payment details will be stored.\",\n      \"type\": \"boolean\"\n    },\n    \"storePaymentMethodMode\": {\n      \"x-addedInVersion\": \"70\",\n      \"description\": \"Indicates if the details of the payment method will be stored for the shopper. Possible values:\\n* **disabled** \\u2013 No details will be stored (default).\\n* **askForConsent** \\u2013 If the `shopperReference` is provided, the UI lets the shopper choose if they want their payment details to be stored.\\n* **enabled** \\u2013 If the `shopperReference` is provided, the details will be stored without asking the shopper for consent.\"\
  ,\n      \"enum\": [\n        \"askForConsent\",\n        \"disabled\",\n        \"enabled\"\n      ],\n      \"type\": \"string\"\n    },\n    \"telephoneNumber\": {\n      \"description\": \"The shopper's telephone number.\",\n      \"type\": \"string\"\n    },\n    \"themeId\": {\n      \"x-addedInVersion\": \"69\",\n      \"description\": \"Sets a custom theme for [Hosted Checkout](https://docs.adyen.com/online-payments/build-your-integration/?platform=Web&integration=Hosted+Checkout). The value can be any of the **Theme ID** values from your Customer Area.\",\n      \"type\": \"string\"\n    },\n    \"threeDSAuthenticationOnly\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"69\",\n      \"x-deprecatedMessage\": \"Use `authenticationData.authenticationOnly` instead.\",\n      \"default\": false,\n      \"description\": \"If set to true, you will only perform the [3D Secure 2 authentication](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only),\
  \ and not the payment authorisation.\",\n      \"type\": \"boolean\"\n    },\n    \"trustedShopper\": {\n      \"description\": \"Set to true if the payment should be routed to a trusted MID.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"amount\",\n    \"reference\",\n    \"returnUrl\",\n    \"merchantAccount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-create-checkout-session-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CreateCheckoutSessionRequest
---
