---
description: Input schema from Adyen API
layout: schema
name: Input
properties_list:
- description: ''
  name: InputCommand
  type: object
- description: ''
  name: ConfirmedFlag
  type: boolean
- description: ''
  name: FunctionKey
  type: integer
- description: ''
  name: TextInput
  type: string
- description: ''
  name: DigitInput
  type: integer
- description: ''
  name: Password
  type: string
- description: ''
  name: MenuEntryNumber
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-input-schema.json
slug: terminal-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-input-schema.json\",\n  \"title\": \"Input\",\n  \"description\": \"Input schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputCommand\": {\n      \"$ref\": \"#/components/schemas/InputCommand\"\n    },\n    \"ConfirmedFlag\": {\n      \"type\": \"boolean\"\n    },\n    \"FunctionKey\": {\n      \"type\": \"integer\"\n    },\n    \"TextInput\": {\n      \"type\": \"string\"\n    },\n    \"DigitInput\": {\n      \"type\": \"integer\"\n    },\n    \"Password\": {\n      \"type\": \"string\"\n    },\n    \"MenuEntryNumber\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    }\n  },\n  \"required\": [\n    \"InputCommand\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-input-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Input
---
