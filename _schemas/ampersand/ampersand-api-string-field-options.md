---
description: Additional options for string fields
layout: schema
name: StringFieldOptions
properties_list:
- description: Maximum length of the string field
  name: length
  type: integer
- description: Regex pattern that the string field value must match
  name: pattern
  type: string
- description: List of allowed values for enum fields
  name: values
  type: array
- description: Indicates if the field value must be limited to what's in Values
  name: valuesRestricted
  type: boolean
- description: Default value for the field
  name: defaultValue
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-string-field-options-schema.json
slug: ampersand-api-string-field-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-string-field-options-schema.json\",\n  \"title\": \"StringFieldOptions\",\n  \"description\": \"Additional options for string fields\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"length\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum length of the string field\"\n    },\n    \"pattern\": {\n      \"type\": \"string\",\n      \"description\": \"Regex pattern that the string field value must match\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"List of allowed values for enum fields\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"valuesRestricted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates if the field value must be limited to what's in Values\"\n    },\n    \"defaultValue\":\
  \ {\n      \"type\": \"string\",\n      \"description\": \"Default value for the field\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-string-field-options-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: StringFieldOptions
---
