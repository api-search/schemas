---
description: Schema for a Search Field
layout: schema
name: SearchField
properties_list:
- description: Merchant api search parameter
  name: searchParameter
  type: string
- description: If the search field is required
  name: required
  type: boolean
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-search-field-schema.json
slug: mastercard-ethoca-merchant-self-services-search-field
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchField\",\n  \"type\": \"object\",\n  \"description\": \"Schema for a Search Field\",\n  \"properties\": {\n    \"searchParameter\": {\n      \"type\": \"string\",\n      \"description\": \"Merchant api search parameter\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"description\": \"If the search field is required\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-search-field-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: SearchField
---
