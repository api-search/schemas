---
description: Request body for creating a new order.
layout: schema
name: OrderCreate
properties_list:
- description: The basket to generate the order from.
  name: basketId
  type: string
- description: The desired output file format. Use the /filetypes endpoint to retrieve supported formats.
  name: fileType
  type: string
provider_name: Moody's
provider_slug: moodys
schema_file: json-schema/moodys-data-buffet-order-create-schema.json
slug: moodys-data-buffet-order-create
source_filename: moodys-data-buffet-order-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrderCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new order.\",\n  \"properties\": {\n    \"basketId\": {\n      \"type\": \"string\",\n      \"description\": \"The basket to generate the order from.\"\n    },\n    \"fileType\": {\n      \"type\": \"string\",\n      \"description\": \"The desired output file format. Use the /filetypes endpoint to retrieve supported formats.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/json-schema/moodys-data-buffet-order-create-schema.json
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
title: OrderCreate
---
