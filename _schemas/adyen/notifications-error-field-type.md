---
description: ErrorFieldType schema from Adyen API
layout: schema
name: ErrorFieldType
properties_list:
- description: The validation error code.
  name: errorCode
  type: integer
- description: A description of the validation error.
  name: errorDescription
  type: string
- description: The type of error field.
  name: fieldType
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notifications-error-field-type-schema.json
slug: notifications-error-field-type
source_filename: notifications-error-field-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-error-field-type-schema.json\",\n  \"title\": \"ErrorFieldType\",\n  \"description\": \"ErrorFieldType schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"description\": \"The validation error code.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"errorDescription\": {\n      \"description\": \"A description of the validation error.\",\n      \"type\": \"string\"\n    },\n    \"fieldType\": {\n      \"description\": \"The type of error field.\",\n      \"$ref\": \"#/components/schemas/FieldType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notifications-error-field-type-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ErrorFieldType
---
