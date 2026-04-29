---
description: ''
layout: schema
name: PatchedAgriculturalMachine
properties_list:
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
  name: hasAgriParcel
  type: string
- description: ''
  name: purchase_date
  type: string
- description: ''
  name: manufacturer
  type: string
- description: ''
  name: model
  type: string
- description: ''
  name: seria_number
  type: string
- description: ''
  name: status
  type: object
- description: ''
  name: invalidatedAtTime
  type: string
- description: ''
  name: dateCreated
  type: string
- description: ''
  name: dateModified
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-patchedagriculturalmachine-schema.json
slug: agstack-openagri-farm-calendar-patchedagriculturalmachine
source_filename: agstack-openagri-farm-calendar-patchedagriculturalmachine-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/PatchedAgriculturalMachine.json\",\n  \"title\": \"PatchedAgriculturalMachine\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"maxLength\": 100\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"hasAgriParcel\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"purchase_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"manufacturer\": {\n      \"type\": \"string\",\n      \"maxLength\": 255\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"maxLength\": 255\n    },\n    \"seria_number\": {\n      \"type\": \"string\",\n      \"maxLength\": 255\n    },\n    \"status\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/StatusEnum\"\n        }\n      ],\n      \"minimum\": -2147483648,\n      \"maximum\": 2147483647\n    },\n    \"invalidatedAtTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"dateModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-patchedagriculturalmachine-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: PatchedAgriculturalMachine
---
