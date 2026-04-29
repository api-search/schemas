---
description: ''
layout: schema
name: YieldPredictionObservation
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
  name: hasArea
  type: string
- description: ''
  name: hasResult
  type: object
- description: ''
  name: observedProperty
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-yieldpredictionobservation-schema.json
slug: agstack-openagri-farm-calendar-yieldpredictionobservation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/YieldPredictionObservation.json\",\n  \"title\": \"YieldPredictionObservation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"activityType\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"maxLength\": 200\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"phenomenonTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"hasEndDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"madeBySensor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MadeBySensorField\"\n        }\n      ],\n      \"nullable\": true\n\
  \    },\n    \"hasAgriParcel\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"hasArea\": {\n      \"type\": \"string\",\n      \"format\": \"decimal\",\n      \"pattern\": \"^-?\\\\d{0,13}(?:\\\\.\\\\d{0,2})?$\"\n    },\n    \"hasResult\": {\n      \"$ref\": \"#/components/schemas/GenericQuantityValueField\"\n    },\n    \"observedProperty\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"activityType\",\n    \"hasAgriParcel\",\n    \"hasArea\",\n    \"hasResult\",\n    \"id\",\n    \"observedProperty\",\n    \"phenomenonTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-yieldpredictionobservation-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: YieldPredictionObservation
---
