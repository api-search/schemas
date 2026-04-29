---
description: POITerminalData schema from Adyen API
layout: schema
name: POITerminalData
properties_list:
- description: ''
  name: TerminalEnvironment
  type: object
- description: ''
  name: POICapabilities
  type: object
- description: ''
  name: POIProfile
  type: object
- description: ''
  name: POISerialNumber
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-poi-terminal-data-schema.json
slug: terminal-poi-terminal-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-poi-terminal-data-schema.json\",\n  \"title\": \"POITerminalData\",\n  \"description\": \"POITerminalData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TerminalEnvironment\": {\n      \"$ref\": \"#/components/schemas/TerminalEnvironment\"\n    },\n    \"POICapabilities\": {\n      \"$ref\": \"#/components/schemas/POICapabilities\"\n    },\n    \"POIProfile\": {\n      \"$ref\": \"#/components/schemas/POIProfile\"\n    },\n    \"POISerialNumber\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    }\n  },\n  \"required\": [\n    \"TerminalEnvironment\",\n    \"POICapabilities\",\n    \"POISerialNumber\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-poi-terminal-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: POITerminalData
---
