---
description: It conveys message text and parameters of the menu entry. This output data could be only provided for an input command, in order to choose an entryof the menu. An entryof the menu to present to the Cashier.
layout: schema
name: MenuEntry
properties_list:
- description: ''
  name: MenuEntryTag
  type: object
- description: ''
  name: DefaultSelectedFlag
  type: boolean
- description: ''
  name: OutputFormat
  type: object
- description: ''
  name: PredefinedContent
  type: object
- description: ''
  name: OutputText
  type: array
- description: ''
  name: OutputXHTML
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-menu-entry-schema.json
slug: terminal-menu-entry
source_filename: terminal-menu-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-menu-entry-schema.json\",\n  \"title\": \"MenuEntry\",\n  \"description\": \"It conveys message text and parameters of the menu entry. This output data could be only provided for an input command, in order to choose an entryof the menu. An entryof the menu to present to the Cashier.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MenuEntryTag\": {\n      \"$ref\": \"#/components/schemas/MenuEntryTag\"\n    },\n    \"DefaultSelectedFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"OutputFormat\": {\n      \"$ref\": \"#/components/schemas/OutputFormat\"\n    },\n    \"PredefinedContent\": {\n      \"$ref\": \"#/components/schemas/PredefinedContent\"\n    },\n    \"OutputText\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/OutputText\"\
  \n      }\n    },\n    \"OutputXHTML\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"pattern\": \"^.+$\"\n    }\n  },\n  \"required\": [\n    \"OutputFormat\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-menu-entry-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MenuEntry
---
