---
description: GetTaxFormResponse schema from Adyen API
layout: schema
name: GetTaxFormResponse
properties_list:
- description: The content of the tax form in Base64 format.
  name: content
  type: string
- description: 'The content type of the tax form. Possible values: * **application/pdf**'
  name: contentType
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-get-tax-form-response-schema.json
slug: configuration-get-tax-form-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-get-tax-form-response-schema.json\",\n  \"title\": \"GetTaxFormResponse\",\n  \"description\": \"GetTaxFormResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"description\": \"The content of the tax form in Base64 format.\",\n      \"format\": \"byte\",\n      \"type\": \"string\"\n    },\n    \"contentType\": {\n      \"description\": \"The content type of the tax form.\\n\\nPossible values:\\n*  **application/pdf**\\n\\n\",\n      \"enum\": [\n        \"application/pdf\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"content\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-get-tax-form-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GetTaxFormResponse
---
