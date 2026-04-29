---
description: Request body for updating a pool.
layout: schema
name: PoolUpdate
properties_list:
- description: ''
  name: description
  type: string
- description: ''
  name: loadBalancingMode
  type: string
- description: ''
  name: monitor
  type: string
- description: ''
  name: serviceDownAction
  type: string
- description: ''
  name: slowRampTime
  type: integer
- description: ''
  name: minActiveMembers
  type: integer
- description: ''
  name: allowNat
  type: string
- description: ''
  name: allowSnat
  type: string
provider_name: F5 Networks
provider_slug: f5-networks
schema_file: json-schema/bigip-icontrol-rest-pool-update-schema.json
slug: bigip-icontrol-rest-pool-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PoolUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a pool.\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"loadBalancingMode\": {\n      \"type\": \"string\"\n    },\n    \"monitor\": {\n      \"type\": \"string\"\n    },\n    \"serviceDownAction\": {\n      \"type\": \"string\"\n    },\n    \"slowRampTime\": {\n      \"type\": \"integer\"\n    },\n    \"minActiveMembers\": {\n      \"type\": \"integer\"\n    },\n    \"allowNat\": {\n      \"type\": \"string\"\n    },\n    \"allowSnat\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/json-schema/bigip-icontrol-rest-pool-update-schema.json
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
title: PoolUpdate
---
