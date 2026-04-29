---
description: UpiCollectDetails schema from Adyen API
layout: schema
name: UpiCollectDetails
properties_list:
- description: The sequence number for the debit. For example, send **2** if this is the second debit for the subscription. The sequence number is included in the notification sent to the shopper.
  name: billingSequenceNumber
  type: string
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: recurringDetailReference
  type: string
- description: The `shopperNotificationReference` returned in the response when you requested to notify the shopper. Used for recurring payment only.
  name: shopperNotificationReference
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: storedPaymentMethodId
  type: string
- description: '**upi_collect**'
  name: type
  type: string
- description: The virtual payment address for UPI.
  name: virtualPaymentAddress
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-upi-collect-details-schema.json
slug: checkout-upi-collect-details
source_filename: checkout-upi-collect-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-upi-collect-details-schema.json\",\n  \"title\": \"UpiCollectDetails\",\n  \"description\": \"UpiCollectDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billingSequenceNumber\": {\n      \"description\": \"The sequence number for the debit. For example, send **2** if this is the second debit for the subscription. The sequence number is included in the notification sent to the shopper.\",\n      \"type\": \"string\"\n    },\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"49\",\n      \"x-deprecatedMessage\": \"Use `storedPaymentMethodId` instead.\",\n \
  \     \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"type\": \"string\"\n    },\n    \"shopperNotificationReference\": {\n      \"description\": \"The `shopperNotificationReference` returned in the response when you requested to notify the shopper. Used for recurring payment only.\",\n      \"type\": \"string\"\n    },\n    \"storedPaymentMethodId\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"maxLength\": 64,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"upi_collect\",\n      \"description\": \"**upi_collect**\",\n      \"enum\": [\n        \"upi_collect\"\n      ],\n      \"type\": \"string\"\n    },\n    \"virtualPaymentAddress\": {\n      \"description\": \"The virtual payment address for UPI.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n\
  \    \"type\",\n    \"billingSequenceNumber\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-upi-collect-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UpiCollectDetails
---
