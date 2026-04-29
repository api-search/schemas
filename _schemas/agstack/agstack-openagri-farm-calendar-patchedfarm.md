---
description: ''
layout: schema
name: PatchedFarm
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: deleted_at
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: administrator
  type: string
- description: ''
  name: telephone
  type: string
- description: ''
  name: vatID
  type: string
- description: ''
  name: hasAgriParcel
  type: array
- description: ''
  name: contactPerson
  type: object
- description: ''
  name: address
  type: object
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-patchedfarm-schema.json
slug: agstack-openagri-farm-calendar-patchedfarm
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/PatchedFarm.json\",\n  \"title\": \"PatchedFarm\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusEnum\"\n        }\n      ],\n      \"minimum\": -2147483648,\n      \"maximum\": 2147483647\n    },\n    \"deleted_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n\
  \    \"administrator\": {\n      \"type\": \"string\"\n    },\n    \"telephone\": {\n      \"type\": \"string\"\n    },\n    \"vatID\": {\n      \"type\": \"string\"\n    },\n    \"hasAgriParcel\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uuid\"\n      },\n      \"readOnly\": true\n    },\n    \"contactPerson\": {\n      \"$ref\": \"#/components/schemas/ContactPersonField\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/AddressField\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-patchedfarm-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: PatchedFarm
---
