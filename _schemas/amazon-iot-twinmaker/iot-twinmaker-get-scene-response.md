---
description: GetSceneResponse schema
layout: schema
name: GetSceneResponse
properties_list:
- description: ''
  name: workspaceId
  type: object
- description: ''
  name: sceneId
  type: object
- description: ''
  name: contentLocation
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: creationDateTime
  type: object
- description: ''
  name: updateDateTime
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
- description: ''
  name: generatedSceneMetadata
  type: object
- description: ''
  name: error
  type: object
provider_name: Amazon IoT TwinMaker
provider_slug: amazon-iot-twinmaker
schema_file: json-schema/iot-twinmaker-get-scene-response-schema.json
slug: iot-twinmaker-get-scene-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-get-scene-response-schema.json\",\n  \"title\": \"GetSceneResponse\",\n  \"description\": \"GetSceneResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workspaceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The ID of the workspace that contains the scene.\"\n        }\n      ]\n    },\n    \"sceneId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The ID of the scene.\"\n        }\n      ]\n    },\n    \"contentLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Url\"\n        },\n        {\n          \"description\": \"The relative path that specifies\
  \ the location of the content definition file.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TwinMakerArn\"\n        },\n        {\n          \"description\": \"The ARN of the scene.\"\n        }\n      ]\n    },\n    \"creationDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the scene was created.\"\n        }\n      ]\n    },\n    \"updateDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the scene was last updated.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the scene.\"\n        }\n      ]\n\
  \    },\n    \"capabilities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SceneCapabilities\"\n        },\n        {\n          \"description\": \"A list of capabilities that the scene uses to render.\"\n        }\n      ]\n    },\n    \"sceneMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SceneMetadataMap\"\n        },\n        {\n          \"description\": \"The response metadata.\"\n        }\n      ]\n    },\n    \"generatedSceneMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GeneratedSceneMetadataMap\"\n        },\n        {\n          \"description\": \"The generated scene metadata.\"\n        }\n      ]\n    },\n    \"error\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SceneError\"\n        },\n        {\n          \"description\": \"The SceneResponse error.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"workspaceId\"\
  ,\n    \"sceneId\",\n    \"contentLocation\",\n    \"arn\",\n    \"creationDateTime\",\n    \"updateDateTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-twinmaker/refs/heads/main/json-schema/iot-twinmaker-get-scene-response-schema.json
tags:
- AWS
- 3D Visualization
- Digital Twin
- Industrial IoT
- IoT
title: GetSceneResponse
---
