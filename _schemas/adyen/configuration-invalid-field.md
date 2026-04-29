---
description: InvalidField schema from Adyen API
layout: schema
name: InvalidField
properties_list:
- description: Description of the validation error.
  name: message
  type: string
- description: The field that has an invalid value.
  name: name
  type: string
- description: The invalid value.
  name: value
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-invalid-field-schema.json
slug: configuration-invalid-field
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-invalid-field-schema.json\",\n  \"title\": \"InvalidField\",\n  \"description\": \"InvalidField schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"description\": \"Description of the validation error.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The field that has an invalid value.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The invalid value.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"value\",\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-invalid-field-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: InvalidField
---
