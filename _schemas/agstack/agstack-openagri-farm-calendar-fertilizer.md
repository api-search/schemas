---
description: ''
layout: schema
name: Fertilizer
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: hasCommercialName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: hasCost
  type: string
- description: ''
  name: isPricePer
  type: string
- description: ''
  name: hasActiveSubstance
  type: string
- description: ''
  name: isTargetedTowards
  type: string
- description: ''
  name: hasNutrientConcentration
  type: string
- description: ''
  name: status
  type: object
- description: ''
  name: dateCreated
  type: string
- description: ''
  name: dateModified
  type: string
- description: ''
  name: invalidatedAtTime
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-fertilizer-schema.json
slug: agstack-openagri-farm-calendar-fertilizer
source_filename: agstack-openagri-farm-calendar-fertilizer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/Fertilizer.json\",\n  \"title\": \"Fertilizer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"hasCommercialName\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"hasCost\": {\n      \"type\": \"string\",\n      \"format\": \"decimal\",\n      \"pattern\": \"^-?\\\\d{0,8}(?:\\\\.\\\\d{0,2})?$\"\n    },\n    \"isPricePer\": {\n      \"type\": \"string\"\n    },\n    \"hasActiveSubstance\": {\n      \"type\": \"string\"\n    },\n    \"isTargetedTowards\": {\n      \"type\": \"string\"\n    },\n    \"hasNutrientConcentration\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusEnum\"\n \
  \       }\n      ],\n      \"minimum\": -2147483648,\n      \"maximum\": 2147483647\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"dateModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"invalidatedAtTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"dateCreated\",\n    \"dateModified\",\n    \"hasActiveSubstance\",\n    \"hasCommercialName\",\n    \"hasCost\",\n    \"hasNutrientConcentration\",\n    \"id\",\n    \"invalidatedAtTime\",\n    \"isPricePer\",\n    \"isTargetedTowards\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-fertilizer-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: Fertilizer
---
