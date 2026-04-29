---
description: CardOrderItemDeliveryStatus schema from Adyen API
layout: schema
name: CardOrderItemDeliveryStatus
properties_list:
- description: An error message.
  name: errorMessage
  type: string
- description: The status of the PIN delivery.
  name: status
  type: string
- description: The tracking number of the PIN delivery.
  name: trackingNumber
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-card-order-item-delivery-status-schema.json
slug: configuration-card-order-item-delivery-status
source_filename: configuration-card-order-item-delivery-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-card-order-item-delivery-status-schema.json\",\n  \"title\": \"CardOrderItemDeliveryStatus\",\n  \"description\": \"CardOrderItemDeliveryStatus schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorMessage\": {\n      \"description\": \"An error message.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the PIN delivery.\",\n      \"enum\": [\n        \"created\",\n        \"delivered\",\n        \"notApplicable\",\n        \"processing\",\n        \"produced\",\n        \"rejected\",\n        \"shipped\",\n        \"unknown\"\n      ],\n      \"type\": \"string\"\n    },\n    \"trackingNumber\": {\n      \"description\": \"The tracking number of the PIN delivery.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-card-order-item-delivery-status-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardOrderItemDeliveryStatus
---
