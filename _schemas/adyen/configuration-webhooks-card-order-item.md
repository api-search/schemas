---
description: CardOrderItem schema from Adyen API
layout: schema
name: CardOrderItem
properties_list:
- description: The unique identifier of the balance platform.
  name: balancePlatform
  type: string
- description: 'The status of the card delivery. Possible values: **created**, **rejected**, **processing**, **produced**, **shipped**, **delivered**, **notApplicable**, **unknown**.'
  name: card
  type: object
- description: The unique identifier of the card order item.
  name: cardOrderItemId
  type: string
- description: The date and time when the event was triggered, in ISO 8601 extended format. For example, **2020-12-18T10:15:30+01:00**.
  name: creationDate
  type: string
- description: The ID of the resource.
  name: id
  type: string
- description: The unique identifier of the payment instrument related to the card order item.
  name: paymentInstrumentId
  type: string
- description: Contains information about the status of the PIN delivery.
  name: pin
  type: object
- description: The shipping method used to deliver the card or the PIN.
  name: shippingMethod
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-webhooks-card-order-item-schema.json
slug: configuration-webhooks-card-order-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-card-order-item-schema.json\",\n  \"title\": \"CardOrderItem\",\n  \"description\": \"CardOrderItem schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balancePlatform\": {\n      \"description\": \"The unique identifier of the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"card\": {\n      \"description\": \"The status of the card delivery.\\n\\nPossible values: **created**, **rejected**, **processing**, **produced**, **shipped**, **delivered**, **notApplicable**, **unknown**. \",\n      \"$ref\": \"#/components/schemas/CardOrderItemDeliveryStatus\"\n    },\n    \"cardOrderItemId\": {\n      \"description\": \"The unique identifier of the card order item.\",\n      \"type\": \"string\"\n    },\n    \"creationDate\": {\n      \"description\": \"The\
  \ date and time when the event was triggered, in ISO 8601 extended format. For example, **2020-12-18T10:15:30+01:00**.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The ID of the resource.\",\n      \"type\": \"string\"\n    },\n    \"paymentInstrumentId\": {\n      \"description\": \"The unique identifier of the payment instrument related to the card order item.\",\n      \"type\": \"string\"\n    },\n    \"pin\": {\n      \"description\": \"Contains information about the status of the PIN delivery.\",\n      \"$ref\": \"#/components/schemas/CardOrderItemDeliveryStatus\"\n    },\n    \"shippingMethod\": {\n      \"description\": \"The shipping method used to deliver the card or the PIN.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-webhooks-card-order-item-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardOrderItem
---
