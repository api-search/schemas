---
description: ''
layout: schema
name: Alert
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
  name: severity
  type: object
- description: ''
  name: hasAgriParcel
  type: string
- description: ''
  name: validFrom
  type: string
- description: ''
  name: validTo
  type: string
- description: ''
  name: dateIssued
  type: string
- description: ''
  name: quantityValue
  type: object
- description: ''
  name: relatedObservation
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-alert-schema.json
slug: agstack-openagri-farm-calendar-alert
source_filename: agstack-openagri-farm-calendar-alert-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/Alert.json\",\n  \"title\": \"Alert\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"activityType\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"maxLength\": 200\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"severity\": {\n      \"$ref\": \"#/components/schemas/SeverityEnum\"\n    },\n    \"hasAgriParcel\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"validFrom\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"validTo\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"dateIssued\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"readOnly\": true,\n      \"nullable\": true\n    },\n    \"quantityValue\": {\n      \"$ref\": \"#/components/schemas/ObservationQuantityValueField\"\n    },\n    \"relatedObservation\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"activityType\",\n    \"dateIssued\",\n    \"hasAgriParcel\",\n    \"id\",\n    \"relatedObservation\",\n    \"validFrom\",\n    \"validTo\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-alert-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: Alert
---
