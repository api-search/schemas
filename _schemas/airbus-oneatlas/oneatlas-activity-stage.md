---
description: ''
layout: schema
name: ActivityStage
properties_list:
- description: Date of the stage
  name: date
  type: string
- description: ''
  name: message
  type: string
- description: Name of the completed stage
  name: name
  type: string
- description: Status of the activity
  name: status
  type: string
- description: ''
  name: userId
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-activity-stage-schema.json
slug: oneatlas-activity-stage
source_filename: oneatlas-activity-stage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-activity-stage-schema.json\",\n  \"title\": \"ActivityStage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"default\": \"now\",\n      \"description\": \"Date of the stage\",\n      \"example\": \"2018-06-12T11:24:31.254Z\",\n      \"format\": \"datetime\",\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Name of the completed stage\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"Status of the activity\",\n      \"enum\": [\n        \"QUEUED\",\n        \"RUNNING\",\n        \"ON_HOLD\",\n        \"CANCELED\",\n        \"WAITING_CANCEL\",\n        \"SUCCEEDED\",\n        \"FAILED\",\n        \"ARCHIVED\"\n      ],\n      \"type\": \"string\"\n   \
  \ },\n    \"userId\": {\n      \"allOf\": [\n        {\n          \"readOnly\": true\n        },\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"If exists, the id of the user that is the origin of the activity stage (extracted from the X-Forwarded-User request header)\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-activity-stage-schema.json
tags:
- Imagery
- Satellites
title: ActivityStage
---
