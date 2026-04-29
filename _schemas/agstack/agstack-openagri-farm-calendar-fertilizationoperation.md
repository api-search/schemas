---
description: ''
layout: schema
name: FertilizationOperation
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
  name: hasApplicationMethod
  type: string
- description: ''
  name: usesFertilizer
  type: string
- description: ''
  name: operatedOn
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-fertilizationoperation-schema.json
slug: agstack-openagri-farm-calendar-fertilizationoperation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/FertilizationOperation.json\",\n  \"title\": \"FertilizationOperation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"activityType\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"maxLength\": 200\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"hasStartDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"hasEndDatetime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"responsibleAgent\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"usesAgriculturalMachinery\": {\n      \"type\": \"array\",\n      \"items\"\
  : {\n        \"type\": \"string\",\n        \"format\": \"uuid\"\n      }\n    },\n    \"hasAppliedAmount\": {\n      \"$ref\": \"#/components/schemas/AppliedAmmountField\"\n    },\n    \"hasApplicationMethod\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"usesFertilizer\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"nullable\": true\n    },\n    \"operatedOn\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    }\n  },\n  \"required\": [\n    \"activityType\",\n    \"hasApplicationMethod\",\n    \"hasAppliedAmount\",\n    \"hasStartDatetime\",\n    \"id\",\n    \"operatedOn\",\n    \"usesAgriculturalMachinery\",\n    \"usesFertilizer\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-fertilizationoperation-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: FertilizationOperation
---
