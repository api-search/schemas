---
description: PlatformPayment schema from Adyen API
layout: schema
name: PlatformPayment
properties_list:
- description: The capture's merchant reference included in the transfer.
  name: modificationMerchantReference
  type: string
- description: The capture reference included in the transfer.
  name: modificationPspReference
  type: string
- description: The payment's merchant reference included in the transfer.
  name: paymentMerchantReference
  type: string
- description: The type of the related split.
  name: platformPaymentType
  type: string
- description: The payment reference included in the transfer.
  name: pspPaymentReference
  type: string
- description: '**platformPayment**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfer-webhooks-platform-payment-schema.json
slug: transfer-webhooks-platform-payment
source_filename: transfer-webhooks-platform-payment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-platform-payment-schema.json\",\n  \"title\": \"PlatformPayment\",\n  \"description\": \"PlatformPayment schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"modificationMerchantReference\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The capture's merchant reference included in the transfer.\",\n      \"type\": \"string\"\n    },\n    \"modificationPspReference\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The capture reference included in the transfer.\",\n      \"type\": \"string\"\n    },\n    \"paymentMerchantReference\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The payment's merchant reference included in the transfer.\",\n      \"type\": \"string\"\n    },\n    \"platformPaymentType\": {\n      \"x-addedInVersion\"\
  : \"4\",\n      \"description\": \"The type of the related split.\",\n      \"enum\": [\n        \"AcquiringFees\",\n        \"AdyenCommission\",\n        \"AdyenFees\",\n        \"AdyenMarkup\",\n        \"BalanceAccount\",\n        \"Commission\",\n        \"Default\",\n        \"Interchange\",\n        \"PaymentFee\",\n        \"Remainder\",\n        \"SchemeFee\",\n        \"TopUp\",\n        \"VAT\"\n      ],\n      \"type\": \"string\"\n    },\n    \"pspPaymentReference\": {\n      \"x-addedInVersion\": \"4\",\n      \"description\": \"The payment reference included in the transfer.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"platformPayment\",\n      \"description\": \"**platformPayment**\",\n      \"enum\": [\n        \"platformPayment\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-platform-payment-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PlatformPayment
---
