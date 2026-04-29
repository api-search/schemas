---
description: ''
layout: schema
name: LinuxParameters
properties_list:
- description: ''
  name: capabilities
  type: object
- description: ''
  name: devices
  type: array
- description: Run an init process inside the container that forwards signals and reaps processes.
  name: initProcessEnabled
  type: boolean
- description: The value for the size (in MiB) of the /dev/shm volume.
  name: sharedMemorySize
  type: integer
- description: ''
  name: tmpfs
  type: array
- description: The total amount of swap memory (in MiB) a container can use.
  name: maxSwap
  type: integer
- description: The container's memory swappiness behavior. A value of 0 prevents swapping; a value of 100 causes pages to be swapped aggressively.
  name: swappiness
  type: integer
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-linux-parameters-schema.json
slug: amazon-ecs-linux-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LinuxParameters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"capabilities\": {\n      \"type\": \"object\"\n    },\n    \"devices\": {\n      \"type\": \"array\"\n    },\n    \"initProcessEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Run an init process inside the container that forwards signals and reaps processes.\"\n    },\n    \"sharedMemorySize\": {\n      \"type\": \"integer\",\n      \"description\": \"The value for the size (in MiB) of the /dev/shm volume.\"\n    },\n    \"tmpfs\": {\n      \"type\": \"array\"\n    },\n    \"maxSwap\": {\n      \"type\": \"integer\",\n      \"description\": \"The total amount of swap memory (in MiB) a container can use.\"\n    },\n    \"swappiness\": {\n      \"type\": \"integer\",\n      \"description\": \"The container's memory swappiness behavior. A value of 0 prevents swapping; a value of 100 causes pages to be swapped\
  \ aggressively.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-linux-parameters-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: LinuxParameters
---
