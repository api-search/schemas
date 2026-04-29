---
description: SceneSummaries schema
layout: schema
name: SceneSummaries
properties_list: []
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-scene-summaries-schema.json
slug: iot-twinmaker-scene-summaries
source_filename: iot-twinmaker-scene-summaries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-scene-summaries-schema.json\",\n  \"title\": \"SceneSummaries\",\n  \"description\": \"SceneSummaries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"sceneId\",\n      \"contentLocation\",\n      \"arn\",\n      \"creationDateTime\",\n      \"updateDateTime\"\n    ],\n    \"properties\": {\n      \"sceneId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Id\"\n          },\n          {\n            \"description\": \"The ID of the scene.\"\n          }\n        ]\n      },\n      \"contentLocation\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/S3Url\"\n          },\n          {\n            \"description\": \"The relative path that specifies the location\
  \ of the content definition file.\"\n          }\n        ]\n      },\n      \"arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TwinMakerArn\"\n          },\n          {\n            \"description\": \"The ARN of the scene.\"\n          }\n        ]\n      },\n      \"creationDateTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The date and time when the scene was created.\"\n          }\n        ]\n      },\n      \"updateDateTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The date and time when the scene was last updated.\"\n          }\n        ]\n      },\n      \"description\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Description\"\n          },\n          {\n            \"description\"\
  : \"The scene description.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An object that contains information about a scene.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-scene-summaries-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: SceneSummaries
---
