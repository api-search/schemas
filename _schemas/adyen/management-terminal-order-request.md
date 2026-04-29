---
description: TerminalOrderRequest schema from Adyen API
layout: schema
name: TerminalOrderRequest
properties_list:
- description: The identification of the billing entity to use for the order.
  name: billingEntityId
  type: string
- description: The merchant-defined purchase order reference.
  name: customerOrderReference
  type: string
- description: The products included in the order.
  name: items
  type: array
- description: Type of order
  name: orderType
  type: string
- description: The identification of the shipping location to use for the order.
  name: shippingLocationId
  type: string
- description: The tax number of the billing entity.
  name: taxId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-order-request-schema.json
slug: management-terminal-order-request
source_filename: management-terminal-order-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-order-request-schema.json\",\n  \"title\": \"TerminalOrderRequest\",\n  \"description\": \"TerminalOrderRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"billingEntityId\": {\n      \"description\": \"The identification of the billing entity to use for the order.\",\n      \"type\": \"string\"\n    },\n    \"customerOrderReference\": {\n      \"description\": \"The merchant-defined purchase order reference.\",\n      \"type\": \"string\"\n    },\n    \"items\": {\n      \"description\": \"The products included in the order.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/OrderItem\"\n      },\n      \"type\": \"array\"\n    },\n    \"orderType\": {\n      \"description\": \"Type of order\",\n      \"type\": \"string\"\n    },\n    \"shippingLocationId\"\
  : {\n      \"description\": \"The identification of the shipping location to use for the order.\",\n      \"type\": \"string\"\n    },\n    \"taxId\": {\n      \"description\": \"The tax number of the billing entity.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-order-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalOrderRequest
---
