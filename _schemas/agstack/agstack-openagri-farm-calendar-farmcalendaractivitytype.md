---
description: ''
layout: schema
name: FarmCalendarActivityType
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
  name: category
  type: object
- description: ''
  name: background_color
  type: string
- description: ''
  name: border_color
  type: string
- description: ''
  name: text_color
  type: string
- description: The farm activitie API endpoint with the specific details of this activity type.
  name: activity_endpoint
  type: string
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-farmcalendaractivitytype-schema.json
slug: agstack-openagri-farm-calendar-farmcalendaractivitytype
source_filename: agstack-openagri-farm-calendar-farmcalendaractivitytype-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/FarmCalendarActivityType.json\",\n  \"title\": \"FarmCalendarActivityType\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"maxLength\": 100\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"category\": {\n      \"$ref\": \"#/components/schemas/CategoryEnum\"\n    },\n    \"background_color\": {\n      \"type\": \"string\",\n      \"pattern\": \"^#[0-9A-Fa-f]{6}$\",\n      \"maxLength\": 7\n    },\n    \"border_color\": {\n      \"type\": \"string\",\n      \"pattern\": \"^#[0-9A-Fa-f]{6}$\",\n      \"maxLength\": 7\n    },\n    \"text_color\": {\n      \"type\": \"string\",\n      \"pattern\": \"^#[0-9A-Fa-f]{6}$\",\n      \"maxLength\": 7\n    },\n    \"\
  activity_endpoint\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"nullable\": true,\n      \"description\": \"The farm activitie API endpoint with the specific details of this activity type.\"\n    }\n  },\n  \"required\": [\n    \"activity_endpoint\",\n    \"id\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-farmcalendaractivitytype-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: FarmCalendarActivityType
---
