---
description: CardOrder schema from Adyen API
layout: schema
name: CardOrder
properties_list:
- description: The date when the card order is created.
  name: beginDate
  type: string
- description: The unique identifier of the card manufacturer profile.
  name: cardManufacturingProfileId
  type: string
- description: The date when the card order processing ends.
  name: closedDate
  type: string
- description: The date when you manually closed the card order. Card orders are automatically closed by the end of the day it was created. If you manually closed it beforehand, the closing date is shown as the `end
  name: endDate
  type: string
- description: The unique identifier of the card order.
  name: id
  type: string
- description: The date when the card order processing begins.
  name: lockDate
  type: string
- description: The service center.
  name: serviceCenter
  type: string
- description: 'The status of the card order. Possible values: **Open**, **Closed**.'
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-card-order-schema.json
slug: configuration-card-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-card-order-schema.json\",\n  \"title\": \"CardOrder\",\n  \"description\": \"CardOrder schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"beginDate\": {\n      \"description\": \"The date when the card order is created.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"cardManufacturingProfileId\": {\n      \"description\": \"The unique identifier of the card manufacturer profile.\",\n      \"type\": \"string\"\n    },\n    \"closedDate\": {\n      \"description\": \"The date when the card order processing ends.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"endDate\": {\n      \"description\": \"The date when you manually closed the card order.\\n\\nCard orders are automatically closed by the end of the day it\
  \ was created. If you manually closed it beforehand, the closing date is shown as the `endDate`.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the card order.\",\n      \"type\": \"string\"\n    },\n    \"lockDate\": {\n      \"description\": \"The date when the card order processing begins.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"serviceCenter\": {\n      \"description\": \"The service center.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the card order.\\n\\nPossible values: **Open**, **Closed**.\",\n      \"enum\": [\n        \"closed\",\n        \"open\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-card-order-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardOrder
---
