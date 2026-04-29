---
description: Request body for creating a new pool.
layout: schema
name: PoolCreate
properties_list:
- description: Name of the pool.
  name: name
  type: string
- description: Administrative partition.
  name: partition
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: loadBalancingMode
  type: string
- description: ''
  name: monitor
  type: string
- description: Initial pool members to add during creation.
  name: members
  type: array
- description: ''
  name: serviceDownAction
  type: string
- description: ''
  name: slowRampTime
  type: integer
- description: ''
  name: allowNat
  type: string
- description: ''
  name: allowSnat
  type: string
provider_name: F5 Networks
provider_slug: f5-networks
schema_file: json-schema/bigip-icontrol-rest-pool-create-schema.json
slug: bigip-icontrol-rest-pool-create
source_filename: bigip-icontrol-rest-pool-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PoolCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new pool.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the pool.\"\n    },\n    \"partition\": {\n      \"type\": \"string\",\n      \"description\": \"Administrative partition.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"loadBalancingMode\": {\n      \"type\": \"string\"\n    },\n    \"monitor\": {\n      \"type\": \"string\"\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"description\": \"Initial pool members to add during creation.\"\n    },\n    \"serviceDownAction\": {\n      \"type\": \"string\"\n    },\n    \"slowRampTime\": {\n      \"type\": \"integer\"\n    },\n    \"allowNat\": {\n      \"type\": \"string\"\n    },\n    \"allowSnat\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/json-schema/bigip-icontrol-rest-pool-create-schema.json
tags:
- API Gateway
- Application Delivery
- Automation
- Edge Computing
- Kubernetes
- Load Balancing
- Multi-Cloud
- NGINX
- Security
- WAF
title: PoolCreate
---
