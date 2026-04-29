---
description: ''
layout: schema
name: ActivitySmall
properties_list:
- description: ''
  name: _links
  type: object
- description: A free text (copy of the last stage message)
  name: message
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-activity-small-schema.json
slug: oneatlas-activity-small
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-activity-small-schema.json\",\n  \"title\": \"ActivitySmall\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_links\": {\n      \"properties\": {\n        \"history\": {\n          \"allOf\": [\n            {\n              \"description\": \"See [Get activity stages](#/paths/~1api~1v1~1activities~1{correlationId}~1stages/get)\"\n            },\n            {\n              \"$ref\": \"#/components/schemas/Link\"\n            }\n          ]\n        },\n        \"monitoring\": {\n          \"allOf\": [\n            {\n              \"description\": \"See [Get activity](#/paths/~1api~1v1~1activities~1{correlationId}/get)\"\n            },\n            {\n              \"$ref\": \"#/components/schemas/Link\"\n            }\n          ]\n        }\n      },\n      \"readOnly\": true,\n   \
  \   \"type\": \"object\"\n    },\n    \"message\": {\n      \"description\": \"A free text (copy of the last stage message)\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-activity-small-schema.json
tags:
- Imagery
- Satellites
title: ActivitySmall
---
