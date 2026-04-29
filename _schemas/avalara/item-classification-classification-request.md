---
description: ClassificationRequest schema from Avalara API
layout: schema
name: ClassificationRequest
properties_list:
- description: ''
  name: items
  type: array
- description: ISO 3166-1 alpha-2 destination country code
  name: destinationCountry
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/item-classification-classification-request-schema.json
slug: item-classification-classification-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/item-classification-classification-request-schema.json\",\n  \"title\": \"ClassificationRequest\",\n  \"description\": \"ClassificationRequest schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"items\"\n  ],\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ClassificationItem\"\n      }\n    },\n    \"destinationCountry\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 destination country code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/item-classification-classification-request-schema.json
tags:
- Taxes
title: ClassificationRequest
---
