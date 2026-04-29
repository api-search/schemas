---
description: ''
layout: schema
name: ActivityStages
properties_list:
- description: ''
  name: data
  type: array
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-activity-stages-schema.json
slug: oneatlas-activity-stages
source_filename: oneatlas-activity-stages-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-activity-stages-schema.json\",\n  \"title\": \"ActivityStages\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ActivityStage\"\n      },\n      \"type\": \"array\",\n      \"uniqueItems\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-activity-stages-schema.json
tags:
- Imagery
- Satellites
title: ActivityStages
---
