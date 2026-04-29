---
description: POISystemData schema from Adyen API
layout: schema
name: POISystemData
properties_list:
- description: ''
  name: DateTime
  type: string
- description: ''
  name: POISoftware
  type: object
- description: ''
  name: POITerminalData
  type: object
- description: ''
  name: POIStatus
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-poi-system-data-schema.json
slug: terminal-poi-system-data
source_filename: terminal-poi-system-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-poi-system-data-schema.json\",\n  \"title\": \"POISystemData\",\n  \"description\": \"POISystemData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"POISoftware\": {\n      \"$ref\": \"#/components/schemas/POISoftware\"\n    },\n    \"POITerminalData\": {\n      \"$ref\": \"#/components/schemas/POITerminalData\"\n    },\n    \"POIStatus\": {\n      \"$ref\": \"#/components/schemas/POIStatus\"\n    }\n  },\n  \"required\": [\n    \"DateTime\",\n    \"POISoftware\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-poi-system-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: POISystemData
---
