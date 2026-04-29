---
description: Merchant Api Search Field
layout: schema
name: SearchFieldResource
properties_list:
- description: Merchant api search parameter
  name: searchParameter
  type: string
- description: Set true if this search parameter is mandatory
  name: required
  type: boolean
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-ethoca-merchant-self-services-search-field-resource-schema.json
slug: mastercard-ethoca-merchant-self-services-search-field-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchFieldResource\",\n  \"type\": \"object\",\n  \"description\": \"Merchant Api Search Field\",\n  \"properties\": {\n    \"searchParameter\": {\n      \"type\": \"string\",\n      \"description\": \"Merchant api search parameter\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Set true if this search parameter is mandatory\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-ethoca-merchant-self-services-search-field-resource-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: SearchFieldResource
---
