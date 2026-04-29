---
description: CreateOrderResponse schema from Adyen API
layout: schema
name: CreateOrderResponse
properties_list:
- description: 'Contains additional information about the payment. Some data fields are included only if you select them first: Go to **Customer Area** > **Developers** > **Additional data**.'
  name: additionalData
  type: object
- description: The initial amount of the order.
  name: amount
  type: object
- description: The date that the order will expire.
  name: expiresAt
  type: string
- description: The fraud result properties of the payment.
  name: fraudResult
  type: object
- description: The encrypted data that will be used by merchant for adding payments to the order.
  name: orderData
  type: string
- description: Adyen's 16-character reference associated with the transaction/request. This value is globally unique; quote it when communicating with us about this request.
  name: pspReference
  type: string
- description: The reference provided by merchant for creating the order.
  name: reference
  type: string
- description: If the payment's authorisation is refused or an error occurs during authorisation, this field holds Adyen's mapped reason for the refusal or a description of the error. When a transaction fails, the a
  name: refusalReason
  type: string
- description: The remaining amount in the order.
  name: remainingAmount
  type: object
- description: The result of the order creation request. The value is always **Success**.
  name: resultCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-create-order-response-schema.json
slug: checkout-create-order-response
source_filename: checkout-create-order-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-create-order-response-schema.json\",\n  \"title\": \"CreateOrderResponse\",\n  \"description\": \"CreateOrderResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"x-anyOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalData3DSecure\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataBillingAddress\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataCard\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataCommon\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataDomesticError\"\n      \
  \  },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataInstallments\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataNetworkTokens\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataOpi\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ResponseAdditionalDataSepa\"\n        }\n      ],\n      \"description\": \"Contains additional information about the payment. Some data fields are included only if you select them first: Go to **Customer Area** > **Developers** > **Additional data**.\",\n      \"type\": \"object\"\n    },\n    \"amount\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The initial amount of the order.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"expiresAt\": {\n      \"description\": \"The date that the order will expire.\",\n      \"type\": \"string\"\n    },\n    \"fraudResult\": {\n      \"description\"\
  : \"The fraud result properties of the payment.\",\n      \"$ref\": \"#/components/schemas/FraudResult\"\n    },\n    \"orderData\": {\n      \"description\": \"The encrypted data that will be used by merchant for adding payments to the order.\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"Adyen's 16-character reference associated with the transaction/request. This value is globally unique; quote it when communicating with us about this request.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"The reference provided by merchant for creating the order.\",\n      \"type\": \"string\"\n    },\n    \"refusalReason\": {\n      \"description\": \"If the payment's authorisation is refused or an error occurs during authorisation, this field holds Adyen's mapped reason for the refusal or a description of the error. When a transaction fails, the authorisation response includes `resultCode` and `refusalReason` values.\\\
  n\\nFor more information, see [Refusal reasons](https://docs.adyen.com/development-resources/refusal-reasons).\",\n      \"type\": \"string\"\n    },\n    \"remainingAmount\": {\n      \"description\": \"The remaining amount in the order.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result of the order creation request.\\n The value is always **Success**.\",\n      \"enum\": [\n        \"Success\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"amount\",\n    \"remainingAmount\",\n    \"expiresAt\",\n    \"orderData\",\n    \"resultCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-create-order-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CreateOrderResponse
---
