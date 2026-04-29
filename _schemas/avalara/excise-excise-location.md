---
description: ExciseLocation schema from Avalara API
layout: schema
name: ExciseLocation
properties_list:
- description: ''
  name: locationId
  type: string
- description: ''
  name: locationName
  type: string
- description: ''
  name: locationType
  type: string
- description: ''
  name: address
  type: object
- description: ''
  name: irsTerminalCode
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/excise-excise-location-schema.json
slug: excise-excise-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-excise-location-schema.json\",\n  \"title\": \"ExciseLocation\",\n  \"description\": \"ExciseLocation schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"locationId\": {\n      \"type\": \"string\"\n    },\n    \"locationName\": {\n      \"type\": \"string\"\n    },\n    \"locationType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Terminal\",\n        \"Warehouse\",\n        \"BulkPlant\",\n        \"Retail\",\n        \"Blender\",\n        \"Refinery\"\n      ]\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/ExciseAddress\"\n    },\n    \"irsTerminalCode\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/excise-excise-location-schema.json
tags:
- Taxes
title: ExciseLocation
---
