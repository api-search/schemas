---
description: ClassifyRequest schema from Avalara API
layout: schema
name: ClassifyRequest
properties_list:
- description: Product description for classification
  name: description
  type: string
- description: ISO 3166-1 alpha-2 destination country
  name: destinationCountry
  type: string
- description: ISO 3166-1 alpha-2 origin country
  name: originCountry
  type: string
- description: Additional product attributes
  name: attributes
  type: object
- description: Product identifier
  name: itemCode
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/hs-code-classification-classify-request-schema.json
slug: hs-code-classification-classify-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/hs-code-classification-classify-request-schema.json\",\n  \"title\": \"ClassifyRequest\",\n  \"description\": \"ClassifyRequest schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"description\",\n    \"destinationCountry\"\n  ],\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Product description for classification\"\n    },\n    \"destinationCountry\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 destination country\"\n    },\n    \"originCountry\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 origin country\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Additional\
  \ product attributes\"\n    },\n    \"itemCode\": {\n      \"type\": \"string\",\n      \"description\": \"Product identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/hs-code-classification-classify-request-schema.json
tags:
- Taxes
title: ClassifyRequest
---
