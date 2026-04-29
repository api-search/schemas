---
description: BalanceCheckResponse schema from Adyen API
layout: schema
name: BalanceCheckResponse
properties_list:
- description: 'Contains additional information about the payment. Some data fields are included only if you select them first: Go to **Customer Area** > **Developers** > **Additional data**.'
  name: additionalData
  type: object
- description: The balance for the payment method.
  name: balance
  type: object
- description: The fraud result properties of the payment.
  name: fraudResult
  type: object
- description: Adyen's 16-character reference associated with the transaction/request. This value is globally unique; quote it when communicating with us about this request.
  name: pspReference
  type: string
- description: If the payment's authorisation is refused or an error occurs during authorisation, this field holds Adyen's mapped reason for the refusal or a description of the error. When a transaction fails, the a
  name: refusalReason
  type: string
- description: 'The result of the cancellation request. Possible values: * **Success** – Indicates that the balance check was successful. * **NotEnoughBalance** – Commonly indicates that the card did not have enough '
  name: resultCode
  type: string
- description: The maximum spendable balance for a single transaction. Applicable to some gift cards.
  name: transactionLimit
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-balance-check-response-schema.json
slug: checkout-balance-check-response
source_filename: checkout-balance-check-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-balance-check-response-schema.json\",\n  \"title\": \"BalanceCheckResponse\",\n  \"description\": \"BalanceCheckResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"x-anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalData3DSecure\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataBillingAddress\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataCard\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataCommon\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataDomesticError\"\n   \
  \     },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataInstallments\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataNetworkTokens\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataOpi\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataSepa\"\n        }\n      ],\n      \"description\": \"Contains additional information about the payment. Some data fields are included only if you select them first: Go to **Customer Area** > **Developers** > **Additional data**.\",\n      \"type\": \"object\"\n    },\n    \"balance\": {\n      \"description\": \"The balance for the payment method.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"fraudResult\": {\n      \"description\": \"The fraud result properties of the payment.\",\n      \"$ref\": \"#/components/schemas/FraudResult\"\n    },\n    \"pspReference\": {\n      \"description\"\
  : \"Adyen's 16-character reference associated with the transaction/request. This value is globally unique; quote it when communicating with us about this request.\",\n      \"type\": \"string\"\n    },\n    \"refusalReason\": {\n      \"description\": \"If the payment's authorisation is refused or an error occurs during authorisation, this field holds Adyen's mapped reason for the refusal or a description of the error. When a transaction fails, the authorisation response includes `resultCode` and `refusalReason` values.\\n\\nFor more information, see [Refusal reasons](https://docs.adyen.com/development-resources/refusal-reasons).\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result of the cancellation request.\\n\\nPossible values:\\n\\n* **Success** \\u2013 Indicates that the balance check was successful.\\n* **NotEnoughBalance** \\u2013 Commonly indicates that the card did not have enough balance to pay the amount in the request, or that\
  \ the currency of the balance on the card did not match the currency of the requested amount.\\n* **Failed** \\u2013 Indicates that the balance check failed.\",\n      \"enum\": [\n        \"Success\",\n        \"NotEnoughBalance\",\n        \"Failed\"\n      ],\n      \"type\": \"string\"\n    },\n    \"transactionLimit\": {\n      \"x-addedInVersion\": \"65\",\n      \"description\": \"The maximum spendable balance for a single transaction. Applicable to some gift cards.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    }\n  },\n  \"required\": [\n    \"balance\",\n    \"resultCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-balance-check-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BalanceCheckResponse
---
