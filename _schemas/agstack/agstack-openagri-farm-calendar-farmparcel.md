---
description: ''
layout: schema
name: FarmParcel
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
  name: identifier
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: validFrom
  type: string
- description: ''
  name: validTo
  type: string
- description: ''
  name: area
  type: string
- description: ''
  name: hasIrrigationFlow
  type: string
- description: ''
  name: category
  type: string
- description: ''
  name: inRegion
  type: string
- description: ''
  name: hasToponym
  type: string
- description: ''
  name: isNitroArea
  type: boolean
- description: ''
  name: isNatura2000Area
  type: boolean
- description: ''
  name: isPdopgArea
  type: boolean
- description: ''
  name: isIrrigated
  type: boolean
- description: ''
  name: isCultivatedInLevels
  type: boolean
- description: ''
  name: isGroundSlope
  type: boolean
- description: ''
  name: depiction
  type: string
- description: ''
  name: hasGeometry
  type: object
- description: ''
  name: location
  type: object
- description: ''
  name: hasAgriCrop
  type: array
- description: ''
  name: farm
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-farmparcel-schema.json
slug: agstack-openagri-farm-calendar-farmparcel
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/FarmParcel.json\",\n  \"title\": \"FarmParcel\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusEnum\"\n        }\n      ],\n      \"minimum\": -2147483648,\n      \"maximum\": 2147483647\n    },\n    \"deleted_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"maxLength\": 255\n    },\n    \"description\": {\n    \
  \  \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"validFrom\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"validTo\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"area\": {\n      \"type\": \"string\",\n      \"format\": \"decimal\",\n      \"pattern\": \"^-?\\\\d{0,13}(?:\\\\.\\\\d{0,2})?$\"\n    },\n    \"hasIrrigationFlow\": {\n      \"type\": \"string\",\n      \"format\": \"decimal\",\n      \"pattern\": \"^-?\\\\d{0,13}(?:\\\\.\\\\d{0,2})?$\",\n      \"nullable\": true\n    },\n    \"category\": {\n      \"type\": \"string\"\n    },\n    \"inRegion\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"hasToponym\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"isNitroArea\": {\n      \"type\": \"boolean\"\n    },\n    \"isNatura2000Area\": {\n      \"type\": \"boolean\"\n    },\n    \"isPdopgArea\": {\n      \"type\": \"boolean\"\n    },\n    \"isIrrigated\"\
  : {\n      \"type\": \"boolean\"\n    },\n    \"isCultivatedInLevels\": {\n      \"type\": \"boolean\"\n    },\n    \"isGroundSlope\": {\n      \"type\": \"boolean\"\n    },\n    \"depiction\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"nullable\": true,\n      \"maxLength\": 500\n    },\n    \"hasGeometry\": {\n      \"$ref\": \"#/components/schemas/GeometrySerializerField\"\n    },\n    \"location\": {\n      \"$ref\": \"#/components/schemas/LocationSerializerField\"\n    },\n    \"hasAgriCrop\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uuid\"\n      },\n      \"readOnly\": true\n    },\n    \"farm\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"created_at\",\n    \"farm\",\n    \"hasAgriCrop\",\n    \"hasGeometry\",\n    \"hasIrrigationFlow\",\n    \"hasToponym\",\n    \"id\",\n    \"identifier\",\n    \"inRegion\",\n    \"isCultivatedInLevels\"\
  ,\n    \"isGroundSlope\",\n    \"isIrrigated\",\n    \"isNatura2000Area\",\n    \"isNitroArea\",\n    \"isPdopgArea\",\n    \"location\",\n    \"updated_at\",\n    \"validFrom\",\n    \"validTo\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-farmparcel-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: FarmParcel
---
