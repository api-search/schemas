---
description: ''
layout: schema
name: AddressField
properties_list:
- description: ''
  name: adminUnitL1
  type: string
- description: ''
  name: adminUnitL2
  type: string
- description: ''
  name: addressArea
  type: string
- description: ''
  name: municipality
  type: string
- description: ''
  name: community
  type: string
- description: ''
  name: locatorName
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-addressfield-schema.json
slug: agstack-openagri-farm-calendar-addressfield
source_filename: agstack-openagri-farm-calendar-addressfield-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/AddressField.json\",\n  \"title\": \"AddressField\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"adminUnitL1\": {\n      \"type\": \"string\"\n    },\n    \"adminUnitL2\": {\n      \"type\": \"string\"\n    },\n    \"addressArea\": {\n      \"type\": \"string\"\n    },\n    \"municipality\": {\n      \"type\": \"string\"\n    },\n    \"community\": {\n      \"type\": \"string\"\n    },\n    \"locatorName\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"addressArea\",\n    \"adminUnitL1\",\n    \"adminUnitL2\",\n    \"community\",\n    \"locatorName\",\n    \"municipality\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-addressfield-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: AddressField
---
