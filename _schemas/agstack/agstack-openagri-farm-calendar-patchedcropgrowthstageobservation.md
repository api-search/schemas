---
description: ''
layout: schema
name: PatchedCropGrowthStageObservation
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: activityType
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: details
  type: string
- description: ''
  name: phenomenonTime
  type: string
- description: ''
  name: hasEndDatetime
  type: string
- description: ''
  name: madeBySensor
  type: object
- description: ''
  name: hasAgriParcel
  type: string
- description: ''
  name: hasAgriCrop
  type: string
- description: ''
  name: hasResult
  type: object
- description: ''
  name: observedProperty
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-patchedcropgrowthstageobservation-schema.json
slug: agstack-openagri-farm-calendar-patchedcropgrowthstageobservation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/PatchedCropGrowthStageObservation.json\",\n  \"title\": \"PatchedCropGrowthStageObservation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"activityType\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"maxLength\": 200\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"phenomenonTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"hasEndDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"madeBySensor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MadeBySensorField\"\n        }\n      ],\n      \"nullable\"\
  : true\n    },\n    \"hasAgriParcel\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"hasAgriCrop\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"hasResult\": {\n      \"$ref\": \"#/components/schemas/GenericQuantityValueField\"\n    },\n    \"observedProperty\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-patchedcropgrowthstageobservation-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: PatchedCropGrowthStageObservation
---
