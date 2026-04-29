---
description: PrintOutput schema from Adyen API
layout: schema
name: PrintOutput
properties_list:
- description: ''
  name: DocumentQualifier
  type: object
- description: ''
  name: ResponseMode
  type: object
- description: ''
  name: IntegratedPrintFlag
  type: boolean
- description: ''
  name: RequiredSignatureFlag
  type: boolean
- description: ''
  name: OutputContent
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-print-output-schema.json
slug: terminal-print-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-print-output-schema.json\",\n  \"title\": \"PrintOutput\",\n  \"description\": \"PrintOutput schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DocumentQualifier\": {\n      \"$ref\": \"#/components/schemas/DocumentQualifier\"\n    },\n    \"ResponseMode\": {\n      \"$ref\": \"#/components/schemas/ResponseMode\"\n    },\n    \"IntegratedPrintFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"RequiredSignatureFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"OutputContent\": {\n      \"$ref\": \"#/components/schemas/OutputContent\"\n    }\n  },\n  \"required\": [\n    \"DocumentQualifier\",\n    \"ResponseMode\",\n    \"OutputContent\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-print-output-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PrintOutput
---
