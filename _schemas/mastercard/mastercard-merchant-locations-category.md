---
description: Merchant Category Name and id
layout: schema
name: Category
properties_list:
- description: The Merchant Category Id
  name: categoryId
  type: string
- description: Name of the category
  name: categoryName
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-merchant-locations-category-schema.json
slug: mastercard-merchant-locations-category
source_filename: mastercard-merchant-locations-category-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Category\",\n  \"type\": \"object\",\n  \"description\": \"Merchant Category Name and id\",\n  \"properties\": {\n    \"categoryId\": {\n      \"type\": \"string\",\n      \"description\": \" The Merchant Category Id\"\n    },\n    \"categoryName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the category\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-merchant-locations-category-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Category
---
