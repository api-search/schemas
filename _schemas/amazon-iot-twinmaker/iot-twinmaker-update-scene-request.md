---
description: UpdateSceneRequest schema
layout: schema
name: UpdateSceneRequest
properties_list:
- description: ''
  name: contentLocation
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: capabilities
  type: object
- description: ''
  name: sceneMetadata
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-update-scene-request-schema.json
slug: iot-twinmaker-update-scene-request
source_filename: iot-twinmaker-update-scene-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-scene-request-schema.json\",\n  \"title\": \"UpdateSceneRequest\",\n  \"description\": \"UpdateSceneRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contentLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Url\"\n        },\n        {\n          \"description\": \"The relative path that specifies the location of the content definition file.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of this scene.\"\n        }\n      ]\n    },\n    \"capabilities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SceneCapabilities\"\n  \
  \      },\n        {\n          \"description\": \"A list of capabilities that the scene uses to render.\"\n        }\n      ]\n    },\n    \"sceneMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SceneMetadataMap\"\n        },\n        {\n          \"description\": \"The scene metadata.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-update-scene-request-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: UpdateSceneRequest
---
