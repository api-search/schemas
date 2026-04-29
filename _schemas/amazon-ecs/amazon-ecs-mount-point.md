---
description: ''
layout: schema
name: MountPoint
properties_list:
- description: The name of the volume to mount.
  name: sourceVolume
  type: string
- description: The path on the container to mount the volume at.
  name: containerPath
  type: string
- description: If this value is true, the container has read-only access to the volume.
  name: readOnly
  type: boolean
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-mount-point-schema.json
slug: amazon-ecs-mount-point
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MountPoint\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceVolume\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the volume to mount.\"\n    },\n    \"containerPath\": {\n      \"type\": \"string\",\n      \"description\": \"The path on the container to mount the volume at.\"\n    },\n    \"readOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"If this value is true, the container has read-only access to the volume.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-mount-point-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: MountPoint
---
