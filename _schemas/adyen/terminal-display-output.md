---
description: It contains a complete display operation for a Display or an Input Device type. For the Input Devices, Diagnosis and EnableService, ResponseRequiredFlag and MinimumDisplayTime shall be absent. Information to display and the way to process the display.
layout: schema
name: DisplayOutput
properties_list:
- description: Request of a message response.
  name: ResponseRequiredFlag
  type: boolean
- description: Number of seconds the message has to be displayed.
  name: MinimumDisplayTime
  type: integer
- description: ''
  name: Device
  type: object
- description: ''
  name: InfoQualify
  type: object
- description: ''
  name: OutputContent
  type: object
- description: ''
  name: MenuEntry
  type: array
- description: If protection has to be provided to the vendor on the text to display or print.
  name: OutputSignature
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-display-output-schema.json
slug: terminal-display-output
source_filename: terminal-display-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-display-output-schema.json\",\n  \"title\": \"DisplayOutput\",\n  \"description\": \"It contains a complete display operation for a Display or an Input Device type. For the Input Devices, Diagnosis and EnableService, ResponseRequiredFlag and MinimumDisplayTime shall be absent. Information to display and the way to process the display.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResponseRequiredFlag\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Request of a message response.\"\n    },\n    \"MinimumDisplayTime\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 999,\n      \"default\": 0,\n      \"description\": \"Number of seconds the message has to be displayed.\"\n    },\n    \"Device\": {\n      \"$ref\": \"#/components/schemas/Device\"\
  \n    },\n    \"InfoQualify\": {\n      \"$ref\": \"#/components/schemas/InfoQualify\"\n    },\n    \"OutputContent\": {\n      \"$ref\": \"#/components/schemas/OutputContent\"\n    },\n    \"MenuEntry\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MenuEntry\"\n      }\n    },\n    \"OutputSignature\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If protection has to be provided to the vendor on the text to display or print.\"\n    }\n  },\n  \"required\": [\n    \"Device\",\n    \"InfoQualify\",\n    \"OutputContent\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-display-output-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DisplayOutput
---
