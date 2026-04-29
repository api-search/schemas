---
description: PaymentFailureNotificationContent schema from Adyen API
layout: schema
name: PaymentFailureNotificationContent
properties_list:
- description: Missing or invalid fields that caused the payment error.
  name: errorFields
  type: array
- description: The error message.
  name: errorMessage
  type: object
- description: The `reference` of the capture or refund.
  name: modificationMerchantReference
  type: string
- description: The `pspReference` of the capture or refund.
  name: modificationPspReference
  type: string
- description: The `reference` of the payment.
  name: paymentMerchantReference
  type: string
- description: The `pspReference` of the payment.
  name: paymentPspReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-payment-failure-notification-content-schema.json
slug: notifications-payment-failure-notification-content
source_filename: notifications-payment-failure-notification-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-payment-failure-notification-content-schema.json\",\n  \"title\": \"PaymentFailureNotificationContent\",\n  \"description\": \"PaymentFailureNotificationContent schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorFields\": {\n      \"description\": \"Missing or invalid fields that caused the payment error.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"errorMessage\": {\n      \"description\": \"The error message.\",\n      \"$ref\": \"#/components/schemas/Message\"\n    },\n    \"modificationMerchantReference\": {\n      \"description\": \"The `reference` of the capture or refund.\",\n      \"type\": \"string\"\n    },\n    \"modificationPspReference\": {\n      \"description\": \"\
  The `pspReference` of the capture or refund.\",\n      \"type\": \"string\"\n    },\n    \"paymentMerchantReference\": {\n      \"description\": \"The `reference` of the payment.\",\n      \"type\": \"string\"\n    },\n    \"paymentPspReference\": {\n      \"description\": \"The `pspReference` of the payment.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-payment-failure-notification-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentFailureNotificationContent
---
