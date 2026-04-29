---
description: Additional options for numeric fields
layout: schema
name: NumericFieldOptions
properties_list:
- description: Total number of digits (for decimal types)
  name: precision
  type: integer
- description: Number of digits to the right of the decimal point (for decimal types)
  name: scale
  type: integer
- description: Minimum value for numeric fields
  name: min
  type: number
- description: Maximum value for numeric fields
  name: max
  type: number
- description: Default value for the field
  name: defaultValue
  type: number
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-numeric-field-options-schema.json
slug: ampersand-api-numeric-field-options
source_filename: ampersand-api-numeric-field-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-numeric-field-options-schema.json\",\n  \"title\": \"NumericFieldOptions\",\n  \"description\": \"Additional options for numeric fields\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"precision\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of digits (for decimal types)\"\n    },\n    \"scale\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of digits to the right of the decimal point (for decimal types)\"\n    },\n    \"min\": {\n      \"type\": \"number\",\n      \"description\": \"Minimum value for numeric fields\"\n    },\n    \"max\": {\n      \"type\": \"number\",\n      \"description\": \"Maximum value for numeric fields\"\n    },\n    \"defaultValue\": {\n      \"type\": \"number\",\n      \"description\": \"Default value for the field\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-numeric-field-options-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: NumericFieldOptions
---
