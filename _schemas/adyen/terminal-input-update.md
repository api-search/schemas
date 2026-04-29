---
description: 'Definition: Content of the Input Update message. : It conveys update of the display of an Input request in progress.'
layout: schema
name: InputUpdate
properties_list:
- description: ''
  name: MessageReference
  type: object
- description: ''
  name: OutputContent
  type: object
- description: ''
  name: MenuEntry
  type: array
- description: ''
  name: OutputSignature
  type: string
- description: ''
  name: MinLength
  type: integer
- description: ''
  name: MaxLength
  type: integer
- description: ''
  name: MaxDecimalLength
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-input-update-schema.json
slug: terminal-input-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-input-update-schema.json\",\n  \"title\": \"InputUpdate\",\n  \"description\": \"Definition: Content of the Input Update message. : It conveys \\t\\t\\t\\tupdate of the display of an Input request in progress.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MessageReference\": {\n      \"$ref\": \"#/components/schemas/MessageReference\"\n    },\n    \"OutputContent\": {\n      \"$ref\": \"#/components/schemas/OutputContent\"\n    },\n    \"MenuEntry\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MenuEntry\"\n      }\n    },\n    \"OutputSignature\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"pattern\": \"^.+$\"\n    },\n    \"MinLength\": {\n      \"type\": \"integer\"\n    },\n    \"MaxLength\": {\n      \"type\": \"integer\"\
  \n    },\n    \"MaxDecimalLength\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"MessageReference\",\n    \"OutputContent\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-input-update-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: InputUpdate
---
