---
description: A coronal mass ejection event from NASA's DONKI space weather database.
layout: schema
name: Coronal Mass Ejection
properties_list:
- description: Unique identifier for the CME event.
  name: activityID
  type: string
- description: Source catalog for the event.
  name: catalog
  type: string
- description: Start time of the CME event.
  name: startTime
  type: string
- description: Location on the Sun where the CME originated.
  name: sourceLocation
  type: string
- description: Active region number on the Sun.
  name: activeRegionNum
  type: integer
- description: Additional notes about the event.
  name: note
  type: string
- description: ''
  name: instruments
  type: array
- description: ''
  name: cmeAnalyses
  type: array
provider_name: NASA
provider_slug: nasa
schema_file: json-schema/coronal-mass-ejection.json
slug: coronal-mass-ejection
source_filename: coronal-mass-ejection.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/nasa/blob/main/json-schema/coronal-mass-ejection.json\",\n  \"title\": \"Coronal Mass Ejection\",\n  \"description\": \"A coronal mass ejection event from NASA's DONKI space weather database.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activityID\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the CME event.\"\n    },\n    \"catalog\": {\n      \"type\": \"string\",\n      \"description\": \"Source catalog for the event.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Start time of the CME event.\"\n    },\n    \"sourceLocation\": {\n      \"type\": \"string\",\n      \"description\": \"Location on the Sun where the CME originated.\"\n    },\n    \"activeRegionNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Active region number\
  \ on the Sun.\"\n    },\n    \"note\": {\n      \"type\": \"string\",\n      \"description\": \"Additional notes about the event.\"\n    },\n    \"instruments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"displayName\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"cmeAnalyses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"time21_5\": { \"type\": \"string\", \"format\": \"date-time\" },\n          \"latitude\": { \"type\": \"number\" },\n          \"longitude\": { \"type\": \"number\" },\n          \"halfAngle\": { \"type\": \"number\" },\n          \"speed\": { \"type\": \"number\" },\n          \"type\": { \"type\": \"string\" },\n          \"isMostAccurate\": { \"type\": \"boolean\" }\n        }\n      }\n    }\n  },\n  \"required\": [\"activityID\", \"startTime\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nasa/refs/heads/main/json-schema/coronal-mass-ejection.json
tags:
- Government
- Science
- Space
title: Coronal Mass Ejection
---
