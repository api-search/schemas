---
description: A saved collection of series requests that can be executed as an order for bulk data retrieval.
layout: schema
name: Basket
properties_list:
- description: Unique identifier for the basket.
  name: basketId
  type: string
- description: User-defined name for the basket.
  name: name
  type: string
- description: Optional description of the basket contents and purpose.
  name: description
  type: string
- description: The series requests contained in the basket.
  name: series
  type: array
- description: When the basket was created.
  name: createdAt
  type: string
- description: When the basket was last modified.
  name: updatedAt
  type: string
provider_name: Moody's
provider_slug: moodys
schema_file: json-schema/moodys-data-buffet-basket-schema.json
slug: moodys-data-buffet-basket
source_filename: moodys-data-buffet-basket-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Basket\",\n  \"type\": \"object\",\n  \"description\": \"A saved collection of series requests that can be executed as an order for bulk data retrieval.\",\n  \"properties\": {\n    \"basketId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the basket.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"User-defined name for the basket.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the basket contents and purpose.\"\n    },\n    \"series\": {\n      \"type\": \"array\",\n      \"description\": \"The series requests contained in the basket.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the basket was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"When the basket was last\
  \ modified.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/json-schema/moodys-data-buffet-basket-schema.json
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
title: Basket
---
