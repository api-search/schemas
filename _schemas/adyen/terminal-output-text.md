---
description: It conveys Information related to the content of the text message and its format. All the data elements related to the format of the text to display or print are parameters valid for the whole Text content. Content of text message to display or print.
layout: schema
name: OutputText
properties_list:
- description: ''
  name: Text
  type: string
- description: ''
  name: CharacterSet
  type: integer
- description: ''
  name: Font
  type: string
- description: ''
  name: StartRow
  type: integer
- description: ''
  name: StartColumn
  type: integer
- description: ''
  name: Color
  type: object
- description: ''
  name: CharacterWidth
  type: object
- description: ''
  name: CharacterHeight
  type: object
- description: ''
  name: CharacterStyle
  type: object
- description: ''
  name: Alignment
  type: object
- description: ''
  name: EndOfLineFlag
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-output-text-schema.json
slug: terminal-output-text
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-output-text-schema.json\",\n  \"title\": \"OutputText\",\n  \"description\": \"It conveys Information related to the content of the text message and its format. All the data elements related to the format of the text to display or print are parameters valid for the whole Text content. Content of text message to display or print.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Text\": {\n      \"type\": \"string\"\n    },\n    \"CharacterSet\": {\n      \"type\": \"integer\"\n    },\n    \"Font\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"StartRow\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 500\n    },\n    \"StartColumn\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 500\n    },\n    \"Color\": {\n \
  \     \"$ref\": \"#/components/schemas/Color\"\n    },\n    \"CharacterWidth\": {\n      \"$ref\": \"#/components/schemas/CharacterWidth\"\n    },\n    \"CharacterHeight\": {\n      \"$ref\": \"#/components/schemas/CharacterHeight\"\n    },\n    \"CharacterStyle\": {\n      \"$ref\": \"#/components/schemas/CharacterStyle\"\n    },\n    \"Alignment\": {\n      \"$ref\": \"#/components/schemas/Alignment\"\n    },\n    \"EndOfLineFlag\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    }\n  },\n  \"required\": [\n    \"Text\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-output-text-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: OutputText
---
