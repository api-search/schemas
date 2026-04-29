---
description: ''
layout: schema
name: ClusterConfiguration
properties_list:
- description: ''
  name: executeCommandConfiguration
  type: object
- description: ''
  name: managedStorageConfiguration
  type: object
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-cluster-configuration-schema.json
slug: amazon-ecs-cluster-configuration
source_filename: amazon-ecs-cluster-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClusterConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"executeCommandConfiguration\": {\n      \"type\": \"object\"\n    },\n    \"managedStorageConfiguration\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-cluster-configuration-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: ClusterConfiguration
---
