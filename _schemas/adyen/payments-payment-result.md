---
description: PaymentResult schema from Adyen API
layout: schema
name: PaymentResult
properties_list:
- description: 'Contains additional information about the payment. Some data fields are included only if you select them first: Go to **Customer Area** > **Developers** > **Additional data**.'
  name: additionalData
  type: object
- description: 'Authorisation code: * When the payment is authorised successfully, this field holds the authorisation code for the payment. * When the payment is not authorised, this field is empty.'
  name: authCode
  type: string
- description: Includes the currency of the conversion and the value of the transaction. > This value only applies if you have implemented Dynamic Currency Conversion. For more information, [contact Support](https:/
  name: dccAmount
  type: object
- description: Cryptographic signature used to verify `dccQuote`. > This value only applies if you have implemented Dynamic Currency Conversion. For more information, [contact Support](https://www.adyen.help/hc/en-u
  name: dccSignature
  type: string
- description: The fraud result properties of the payment.
  name: fraudResult
  type: object
- description: The URL to direct the shopper to. > In case of SecurePlus, do not redirect a shopper to this URL.
  name: issuerUrl
  type: string
- description: The payment session.
  name: md
  type: string
- description: 'The 3D request data for the issuer. If the value is **CUPSecurePlus-CollectSMSVerificationCode**, collect an SMS code from the shopper and pass it in the `/authorise3D` request. For more information, '
  name: paRequest
  type: string
- description: Adyen's 16-character reference associated with the transaction/request. This value is globally unique; quote it when communicating with us about this request.
  name: pspReference
  type: string
- description: If the payment's authorisation is refused or an error occurs during authorisation, this field holds Adyen's mapped reason for the refusal or a description of the error. When a transaction fails, the a
  name: refusalReason
  type: string
- description: 'The result of the payment. For more information, see [Result codes](https://docs.adyen.com/online-payments/payment-result-codes). Possible values: * **AuthenticationFinished** – The payment has been s'
  name: resultCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-payment-result-schema.json
slug: payments-payment-result
source_filename: payments-payment-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-payment-result-schema.json\",\n  \"title\": \"PaymentResult\",\n  \"description\": \"PaymentResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"x-anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalData3DSecure\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataBillingAddress\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataCard\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataCommon\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataDomesticError\"\n        },\n        {\n  \
  \        \"$ref\": \"#/components/schemas/ResponseAdditionalDataInstallments\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataNetworkTokens\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataOpi\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataSepa\"\n        }\n      ],\n      \"description\": \"Contains additional information about the payment. Some data fields are included only if you select them first: Go to **Customer Area** > **Developers** > **Additional data**.\",\n      \"type\": \"object\"\n    },\n    \"authCode\": {\n      \"description\": \"Authorisation code:\\n* When the payment is authorised successfully, this field holds the authorisation code for the payment.\\n* When the payment is not authorised, this field is empty.\",\n      \"type\": \"string\"\n    },\n    \"dccAmount\": {\n      \"description\": \"Includes the currency of the conversion and\
  \ the value of the transaction.\\n> This value only applies if you have implemented Dynamic Currency Conversion. For more information, [contact Support](https://www.adyen.help/hc/en-us/requests/new).\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"dccSignature\": {\n      \"description\": \"Cryptographic signature used to verify `dccQuote`.\\n> This value only applies if you have implemented Dynamic Currency Conversion. For more information, [contact Support](https://www.adyen.help/hc/en-us/requests/new).\",\n      \"type\": \"string\"\n    },\n    \"fraudResult\": {\n      \"description\": \"The fraud result properties of the payment.\",\n      \"$ref\": \"#/components/schemas/FraudResult\"\n    },\n    \"issuerUrl\": {\n      \"description\": \"The URL to direct the shopper to.\\n> In case of SecurePlus, do not redirect a shopper to this URL.\",\n      \"type\": \"string\"\n    },\n    \"md\": {\n      \"description\": \"The payment session.\",\n      \"maxLength\"\
  : 20000,\n      \"type\": \"string\"\n    },\n    \"paRequest\": {\n      \"description\": \"The 3D request data for the issuer.\\n\\nIf the value is **CUPSecurePlus-CollectSMSVerificationCode**, collect an SMS code from the shopper and pass it in the `/authorise3D` request. For more information, see [3D Secure](https://docs.adyen.com/classic-integration/3d-secure).\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"Adyen's 16-character reference associated with the transaction/request. This value is globally unique; quote it when communicating with us about this request.\",\n      \"type\": \"string\"\n    },\n    \"refusalReason\": {\n      \"description\": \"If the payment's authorisation is refused or an error occurs during authorisation, this field holds Adyen's mapped reason for the refusal or a description of the error. When a transaction fails, the authorisation response includes `resultCode` and `refusalReason` values.\\n\\nFor more information,\
  \ see [Refusal reasons](https://docs.adyen.com/development-resources/refusal-reasons).\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result of the payment. For more information, see [Result codes](https://docs.adyen.com/online-payments/payment-result-codes).\\n\\nPossible values:\\n\\n* **AuthenticationFinished** \\u2013 The payment has been successfully authenticated with 3D Secure 2. Returned for 3D Secure 2 authentication-only transactions.\\n* **AuthenticationNotRequired** \\u2013 The transaction does not require 3D Secure authentication. Returned for [standalone authentication-only integrations](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only).\\n* **Authorised** \\u2013 The payment was successfully authorised. This state serves as an indicator to proceed with the delivery of goods and services. This is a final state.\\n* **Cancelled** \\u2013 Indicates the payment has been cancelled (either by the\
  \ shopper or the merchant) before processing was completed. This is a final state.\\n* **ChallengeShopper** \\u2013 The issuer requires further shopper interaction before the payment can be authenticated. Returned for 3D Secure 2 transactions.\\n* **Error** \\u2013 There was an error when the payment was being processed. The reason is given in the `refusalReason` field. This is a final state.\\n* **IdentifyShopper** \\u2013 The issuer requires the shopper's device fingerprint before the payment can be authenticated. Returned for 3D Secure 2 transactions.\\n* **PartiallyAuthorised** \\u2013 The payment has been authorised for a partial amount.\\nThis happens for card payments when the merchant supports Partial Authorisations and the cardholder has insufficient funds.\\n* **Pending** \\u2013 Indicates that it is not possible to obtain the final status of the payment. This can happen if the systems providing final status information for the payment are unavailable, or if the shopper needs\
  \ to take further action to complete the payment.\\n* **PresentToShopper** \\u2013 Indicates that the response contains additional information that you need to present to a shopper, so that they can use it to complete a payment.\\n* **Received** \\u2013 Indicates the payment has successfully been received by Adyen, and will be processed. This is the initial state for all payments.\\n* **RedirectShopper** \\u2013 Indicates the shopper should be redirected to an external web page or app to complete the authorisation.\\n* **Refused** \\u2013 Indicates the payment was refused. The reason is given in the `refusalReason` field. This is a final state.\",\n      \"enum\": [\n        \"AuthenticationFinished\",\n        \"AuthenticationNotRequired\",\n        \"Authorised\",\n        \"Cancelled\",\n        \"ChallengeShopper\",\n        \"Error\",\n        \"IdentifyShopper\",\n        \"PartiallyAuthorised\",\n        \"Pending\",\n        \"PresentToShopper\",\n        \"Received\",\n      \
  \  \"RedirectShopper\",\n        \"Refused\",\n        \"Success\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-payment-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentResult
---
