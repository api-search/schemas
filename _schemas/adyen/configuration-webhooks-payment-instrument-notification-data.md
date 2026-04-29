---
description: PaymentInstrumentNotificationData schema from Adyen API
layout: schema
name: PaymentInstrumentNotificationData
properties_list:
- description: The unique identifier of the balance platform.
  name: balancePlatform
  type: string
- description: Contains information about the payment instrument resource that triggered the event.
  name: paymentInstrument
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-payment-instrument-notification-data-schema.json
slug: configuration-webhooks-payment-instrument-notification-data
source_filename: configuration-webhooks-payment-instrument-notification-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-payment-instrument-notification-data-schema.json\",\n  \"title\": \"PaymentInstrumentNotificationData\",\n  \"description\": \"PaymentInstrumentNotificationData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balancePlatform\": {\n      \"description\": \"The unique identifier of the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"paymentInstrument\": {\n      \"description\": \"Contains information about the payment instrument resource that triggered the event.\",\n      \"$ref\": \"#/components/schemas/PaymentInstrument\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-payment-instrument-notification-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentInstrumentNotificationData
---
