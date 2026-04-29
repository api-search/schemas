---
description: BusinessLines schema from Adyen API
layout: schema
name: BusinessLines
properties_list:
- description: List of business lines.
  name: businessLines
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/legal-entity-business-lines-schema.json
slug: legal-entity-business-lines
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-business-lines-schema.json\",\n  \"title\": \"BusinessLines\",\n  \"description\": \"BusinessLines schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"businessLines\": {\n      \"description\": \"List of business lines.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BusinessLine\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"businessLines\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/legal-entity-business-lines-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BusinessLines
---
