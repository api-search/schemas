---
description: ''
layout: schema
name: Volume
properties_list:
- description: The name of the volume (up to 255 characters).
  name: name
  type: string
- description: The contents of the host parameter determine whether your data volume persists on the host container instance.
  name: host
  type: object
- description: ''
  name: dockerVolumeConfiguration
  type: object
- description: ''
  name: efsVolumeConfiguration
  type: object
- description: ''
  name: fsxWindowsFileServerVolumeConfiguration
  type: object
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-volume-schema.json
slug: amazon-ecs-volume
source_filename: amazon-ecs-volume-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Volume\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the volume (up to 255 characters).\"\n    },\n    \"host\": {\n      \"type\": \"object\",\n      \"description\": \"The contents of the host parameter determine whether your data volume persists on the host container instance.\"\n    },\n    \"dockerVolumeConfiguration\": {\n      \"type\": \"object\"\n    },\n    \"efsVolumeConfiguration\": {\n      \"type\": \"object\"\n    },\n    \"fsxWindowsFileServerVolumeConfiguration\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-volume-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: Volume
---
