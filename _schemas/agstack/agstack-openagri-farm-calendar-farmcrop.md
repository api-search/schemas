---
description: ''
layout: schema
name: FarmCrop
properties_list:
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
  name: cropSpecies
  type: object
- description: ''
  name: growth_stage
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-farmcrop-schema.json
slug: agstack-openagri-farm-calendar-farmcrop
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/FarmCrop.json\",\n  \"title\": \"FarmCrop\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusEnum\"\n        }\n      ],\n      \"minimum\": -2147483648,\n      \"maximum\": 2147483647\n    },\n    \"invalidatedAtTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"dateModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"maxLength\": 100\n    },\n    \"description\": {\n    \
  \  \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"hasAgriParcel\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"cropSpecies\": {\n      \"$ref\": \"#/components/schemas/CropSpeciesSerializerField\"\n    },\n    \"growth_stage\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 255\n    }\n  },\n  \"required\": [\n    \"cropSpecies\",\n    \"dateCreated\",\n    \"dateModified\",\n    \"hasAgriParcel\",\n    \"id\",\n    \"invalidatedAtTime\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-farmcrop-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: FarmCrop
---
