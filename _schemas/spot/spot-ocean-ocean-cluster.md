---
description: ''
layout: schema
name: OceanCluster
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: controllerClusterId
  type: string
- description: ''
  name: region
  type: string
- description: ''
  name: autoScaler
  type: object
- description: ''
  name: capacity
  type: object
- description: ''
  name: strategy
  type: object
- description: ''
  name: compute
  type: object
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Spot
provider_slug: spot
schema_file: json-schema/spot-ocean-ocean-cluster-schema.json
slug: spot-ocean-ocean-cluster
source_filename: spot-ocean-ocean-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OceanCluster\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"controllerClusterId\": {\n      \"type\": \"string\"\n    },\n    \"region\": {\n      \"type\": \"string\"\n    },\n    \"autoScaler\": {\n      \"type\": \"object\"\n    },\n    \"capacity\": {\n      \"type\": \"object\"\n    },\n    \"strategy\": {\n      \"type\": \"object\"\n    },\n    \"compute\": {\n      \"type\": \"object\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/json-schema/spot-ocean-ocean-cluster-schema.json
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
title: OceanCluster
---
