---
description: PaymentResponse schema from Adyen API
layout: schema
name: PaymentResponse
properties_list:
- description: Action to be taken for completing the payment.
  name: action
  type: object
- description: 'Contains additional information about the payment. Some data fields are included only if you select them first: Go to **Customer Area** > **Developers** > **Additional data**.'
  name: additionalData
  type: object
- description: Authorised amount in the transaction.
  name: amount
  type: object
- description: Donation Token containing payment details for Adyen Giving.
  name: donationToken
  type: string
- description: The fraud result properties of the payment.
  name: fraudResult
  type: object
- description: The reference to uniquely identify a payment. This reference is used in all communication with you about the payment status. We recommend using a unique value per payment; however, it is not a require
  name: merchantReference
  type: string
- description: Contains updated information regarding the order in case order information was provided in the request.
  name: order
  type: object
- description: Details about the payment method used in the transaction. Only returned if `resultCode` is **Authorised**.
  name: paymentMethod
  type: object
- description: Adyen's 16-character string reference associated with the transaction/request. This value is globally unique; quote it when communicating with us about this request. > For payment methods that require
  name: pspReference
  type: string
- description: If the payment's authorisation is refused or an error occurs during authorisation, this field holds Adyen's mapped reason for the refusal or a description of the error. When a transaction fails, the a
  name: refusalReason
  type: string
- description: Code that specifies the refusal reason. For more information, see [Authorisation refusal reasons](https://docs.adyen.com/development-resources/refusal-reasons).
  name: refusalReasonCode
  type: string
- description: 'The result of the payment. For more information, see [Result codes](https://docs.adyen.com/online-payments/payment-result-codes). Possible values: * **AuthenticationFinished** – The payment has been s'
  name: resultCode
  type: string
- description: Response of the 3D Secure 2 authentication.
  name: threeDS2ResponseData
  type: object
- description: Result of the 3D Secure 2 authentication.
  name: threeDS2Result
  type: object
- description: When non-empty, contains a value that you must submit to the `/payments/details` endpoint as `paymentData`.
  name: threeDSPaymentData
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-payment-response-schema.json
slug: checkout-payment-response
source_filename: checkout-payment-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-response-schema.json\",\n  \"title\": \"PaymentResponse\",\n  \"description\": \"PaymentResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"Action to be taken for completing the payment.\",\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CheckoutAwaitAction\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/CheckoutDelegatedAuthenticationAction\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/CheckoutNativeRedirectAction\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/CheckoutQrCodeAction\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/CheckoutRedirectAction\"\n        },\n        {\n\
  \          \"$ref\": \"#/components/schemas/CheckoutSDKAction\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/CheckoutThreeDS2Action\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/CheckoutVoucherAction\"\n        }\n      ]\n    },\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"x-anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalData3DSecure\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataBillingAddress\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataCard\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataCommon\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataDomesticError\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataInstallments\"\n  \
  \      },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataNetworkTokens\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataOpi\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataSepa\"\n        }\n      ],\n      \"description\": \"Contains additional information about the payment. Some data fields are included only if you select them first: Go to **Customer Area** > **Developers** > **Additional data**.\",\n      \"type\": \"object\"\n    },\n    \"amount\": {\n      \"x-addedInVersion\": \"52\",\n      \"description\": \"Authorised amount in the transaction.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"donationToken\": {\n      \"x-addedInVersion\": \"66\",\n      \"description\": \"Donation Token containing payment details for Adyen Giving.\",\n      \"type\": \"string\"\n    },\n    \"fraudResult\": {\n      \"description\": \"The fraud result properties\
  \ of the payment.\",\n      \"$ref\": \"#/components/schemas/FraudResult\"\n    },\n    \"merchantReference\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"The reference to uniquely identify a payment. This reference is used in all communication with you about the payment status. We recommend using a unique value per payment; however, it is not a requirement.\\nIf you need to provide multiple references for a transaction, separate them with hyphens (\\\"-\\\").\\nMaximum length: 80 characters.\",\n      \"type\": \"string\"\n    },\n    \"order\": {\n      \"description\": \"Contains updated information regarding the order in case order information was provided in the request.\",\n      \"$ref\": \"#/components/schemas/CheckoutOrderResponse\"\n    },\n    \"paymentMethod\": {\n      \"x-addedInVersion\": \"69\",\n      \"description\": \"Details about the payment method used in the transaction. \\nOnly returned if `resultCode` is **Authorised**.\",\n      \"$ref\":\
  \ \"#/components/schemas/ResponsePaymentMethod\"\n    },\n    \"pspReference\": {\n      \"description\": \"Adyen's 16-character string reference associated with the transaction/request. This value is globally unique; quote it when communicating with us about this request.\\n\\n> For payment methods that require a redirect or additional action, you will get this value in the `/payments/details` response.\",\n      \"type\": \"string\"\n    },\n    \"refusalReason\": {\n      \"description\": \"If the payment's authorisation is refused or an error occurs during authorisation, this field holds Adyen's mapped reason for the refusal or a description of the error. When a transaction fails, the authorisation response includes `resultCode` and `refusalReason` values.\\n\\nFor more information, see [Refusal reasons](https://docs.adyen.com/development-resources/refusal-reasons).\",\n      \"type\": \"string\"\n    },\n    \"refusalReasonCode\": {\n      \"x-addedInVersion\": \"37\",\n      \"description\"\
  : \"Code that specifies the refusal reason. For more information, see [Authorisation refusal reasons](https://docs.adyen.com/development-resources/refusal-reasons).\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result of the payment. For more information, see [Result codes](https://docs.adyen.com/online-payments/payment-result-codes).\\n\\nPossible values:\\n\\n* **AuthenticationFinished** \\u2013 The payment has been successfully authenticated with 3D Secure 2. Returned for 3D Secure 2 authentication-only transactions.\\n* **AuthenticationNotRequired** \\u2013 The transaction does not require 3D Secure authentication. Returned for [standalone authentication-only integrations](https://docs.adyen.com/online-payments/3d-secure/other-3ds-flows/authentication-only).\\n* **Authorised** \\u2013 The payment was successfully authorised. This state serves as an indicator to proceed with the delivery of goods and services. This is a final state.\\n*\
  \ **Cancelled** \\u2013 Indicates the payment has been cancelled (either by the shopper or the merchant) before processing was completed. This is a final state.\\n* **ChallengeShopper** \\u2013 The issuer requires further shopper interaction before the payment can be authenticated. Returned for 3D Secure 2 transactions.\\n* **Error** \\u2013 There was an error when the payment was being processed. The reason is given in the `refusalReason` field. This is a final state.\\n* **IdentifyShopper** \\u2013 The issuer requires the shopper's device fingerprint before the payment can be authenticated. Returned for 3D Secure 2 transactions.\\n* **PartiallyAuthorised** \\u2013 The payment has been authorised for a partial amount.\\nThis happens for card payments when the merchant supports Partial Authorisations and the cardholder has insufficient funds.\\n* **Pending** \\u2013 Indicates that it is not possible to obtain the final status of the payment. This can happen if the systems providing final\
  \ status information for the payment are unavailable, or if the shopper needs to take further action to complete the payment.\\n* **PresentToShopper** \\u2013 Indicates that the response contains additional information that you need to present to a shopper, so that they can use it to complete a payment.\\n* **Received** \\u2013 Indicates the payment has successfully been received by Adyen, and will be processed. This is the initial state for all payments.\\n* **RedirectShopper** \\u2013 Indicates the shopper should be redirected to an external web page or app to complete the authorisation.\\n* **Refused** \\u2013 Indicates the payment was refused. The reason is given in the `refusalReason` field. This is a final state.\",\n      \"enum\": [\n        \"AuthenticationFinished\",\n        \"AuthenticationNotRequired\",\n        \"Authorised\",\n        \"Cancelled\",\n        \"ChallengeShopper\",\n        \"Error\",\n        \"IdentifyShopper\",\n        \"PartiallyAuthorised\",\n      \
  \  \"Pending\",\n        \"PresentToShopper\",\n        \"Received\",\n        \"RedirectShopper\",\n        \"Refused\",\n        \"Success\"\n      ],\n      \"type\": \"string\"\n    },\n    \"threeDS2ResponseData\": {\n      \"x-addedInVersion\": \"67\",\n      \"description\": \"Response of the 3D Secure 2 authentication.\",\n      \"$ref\": \"#/components/schemas/ThreeDS2ResponseData\"\n    },\n    \"threeDS2Result\": {\n      \"x-addedInVersion\": \"41\",\n      \"description\": \"Result of the 3D Secure 2 authentication.\",\n      \"$ref\": \"#/components/schemas/ThreeDS2Result\"\n    },\n    \"threeDSPaymentData\": {\n      \"x-addedInVersion\": \"67\",\n      \"description\": \"When non-empty, contains a value that you must submit to the `/payments/details` endpoint as `paymentData`.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-payment-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentResponse
---
