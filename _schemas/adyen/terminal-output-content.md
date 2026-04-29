---
description: This is a sequence of elements if they have different formats. Content to display or print.
layout: schema
name: OutputContent
properties_list:
- description: ''
  name: OutputFormat
  type: object
- description: ''
  name: PredefinedContent
  type: object
- description: ''
  name: OutputText
  type: array
- description: Mandatory, if OutputFormat is XHTML, not allowed otherwise.
  name: OutputXHTML
  type: string
- description: ''
  name: OutputBarcode
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-output-content-schema.json
slug: terminal-output-content
source_filename: terminal-output-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-output-content-schema.json\",\n  \"title\": \"OutputContent\",\n  \"description\": \"This is a sequence of elements if they have different formats. Content to display or print.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutputFormat\": {\n      \"$ref\": \"#/components/schemas/OutputFormat\"\n    },\n    \"PredefinedContent\": {\n      \"$ref\": \"#/components/schemas/PredefinedContent\"\n    },\n    \"OutputText\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/OutputText\"\n      }\n    },\n    \"OutputXHTML\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"pattern\": \"^.{0,262144}$\",\n      \"description\": \"Mandatory, if OutputFormat is XHTML, not allowed otherwise.\"\n    },\n    \"OutputBarcode\": {\n      \"$ref\"\
  : \"#/components/schemas/OutputBarcode\"\n    }\n  },\n  \"required\": [\n    \"OutputFormat\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-output-content-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: OutputContent
---
