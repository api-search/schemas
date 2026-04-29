---
description: A data generation order created from a basket. Orders are processed asynchronously and produce downloadable output files.
layout: schema
name: Order
properties_list:
- description: Unique identifier for the order.
  name: orderId
  type: string
- description: The basket from which the order was generated.
  name: basketId
  type: string
- description: Current processing status of the order.
  name: status
  type: string
- description: The output file format for the order.
  name: fileType
  type: string
- description: When the order was created.
  name: createdAt
  type: string
- description: When the order processing completed.
  name: completedAt
  type: string
- description: URL to download the order output. Available only when status is Complete.
  name: downloadUrl
  type: string
- description: Error description if the order failed. Present only when status is Failed.
  name: errorMessage
  type: string
provider_name: Moody's
provider_slug: moodys
schema_file: json-schema/moodys-data-buffet-order-schema.json
slug: moodys-data-buffet-order
source_filename: moodys-data-buffet-order-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Order\",\n  \"type\": \"object\",\n  \"description\": \"A data generation order created from a basket. Orders are processed asynchronously and produce downloadable output files.\",\n  \"properties\": {\n    \"orderId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the order.\"\n    },\n    \"basketId\": {\n      \"type\": \"string\",\n      \"description\": \"The basket from which the order was generated.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current processing status of the order.\"\n    },\n    \"fileType\": {\n      \"type\": \"string\",\n      \"description\": \"The output file format for the order.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the order was created.\"\n    },\n    \"completedAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the\
  \ order processing completed.\"\n    },\n    \"downloadUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL to download the order output. Available only when status is Complete.\"\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Error description if the order failed. Present only when status is Failed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/json-schema/moodys-data-buffet-order-schema.json
tags:
- Climate Risk
- Compliance
- Credit Risk
- Economic Data
- Entity Verification
- Financial Analytics
- Insurance
- KYC
- Risk
- Screening
title: Order
---
