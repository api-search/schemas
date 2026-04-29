---
description: ''
layout: schema
name: IrrigationOperation
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
  name: hasStartDatetime
  type: string
- description: ''
  name: hasEndDatetime
  type: string
- description: ''
  name: responsibleAgent
  type: string
- description: ''
  name: usesAgriculturalMachinery
  type: array
- description: ''
  name: hasAppliedAmount
  type: object
- description: ''
  name: usesIrrigationSystem
  type: object
- description: ''
  name: operatedOn
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-irrigationoperation-schema.json
slug: agstack-openagri-farm-calendar-irrigationoperation
source_filename: agstack-openagri-farm-calendar-irrigationoperation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/IrrigationOperation.json\",\n  \"title\": \"IrrigationOperation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"activityType\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"maxLength\": 200\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"hasStartDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"hasEndDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"responsibleAgent\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"usesAgriculturalMachinery\": {\n      \"type\": \"array\",\n      \"items\": {\n \
  \       \"type\": \"string\",\n        \"format\": \"uuid\"\n      }\n    },\n    \"hasAppliedAmount\": {\n      \"$ref\": \"#/components/schemas/AppliedAmmountField\"\n    },\n    \"usesIrrigationSystem\": {\n      \"$ref\": \"#/components/schemas/UsesIrrigationSystemEnum\"\n    },\n    \"operatedOn\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    }\n  },\n  \"required\": [\n    \"activityType\",\n    \"hasAppliedAmount\",\n    \"hasStartDatetime\",\n    \"id\",\n    \"operatedOn\",\n    \"usesAgriculturalMachinery\",\n    \"usesIrrigationSystem\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-irrigationoperation-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: IrrigationOperation
---
