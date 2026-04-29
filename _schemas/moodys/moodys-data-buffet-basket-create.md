---
description: Request body for creating or updating a basket.
layout: schema
name: BasketCreate
properties_list:
- description: User-defined name for the basket.
  name: name
  type: string
- description: Optional description of the basket.
  name: description
  type: string
- description: The series requests to include in the basket.
  name: series
  type: array
provider_name: Moody's
provider_slug: moodys
schema_file: json-schema/moodys-data-buffet-basket-create-schema.json
slug: moodys-data-buffet-basket-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BasketCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating or updating a basket.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"User-defined name for the basket.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description of the basket.\"\n    },\n    \"series\": {\n      \"type\": \"array\",\n      \"description\": \"The series requests to include in the basket.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/json-schema/moodys-data-buffet-basket-create-schema.json
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
title: BasketCreate
---
