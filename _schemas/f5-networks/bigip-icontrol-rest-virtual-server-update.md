---
description: Request body for updating a virtual server.
layout: schema
name: VirtualServerUpdate
properties_list:
- description: ''
  name: description
  type: string
- description: ''
  name: destination
  type: string
- description: ''
  name: ipProtocol
  type: string
- description: ''
  name: mask
  type: string
- description: ''
  name: pool
  type: string
- description: ''
  name: profiles
  type: array
- description: ''
  name: persist
  type: array
- description: ''
  name: source
  type: string
- description: ''
  name: sourcePort
  type: string
- description: ''
  name: translateAddress
  type: string
- description: ''
  name: translatePort
  type: string
- description: ''
  name: connectionLimit
  type: integer
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: disabled
  type: boolean
- description: ''
  name: mirror
  type: string
- description: ''
  name: rateLimit
  type: string
- description: ''
  name: rules
  type: array
- description: ''
  name: vlans
  type: array
- description: ''
  name: vlansEnabled
  type: boolean
- description: ''
  name: vlansDisabled
  type: boolean
- description: ''
  name: fallbackPersistence
  type: string
provider_name: F5 Networks
provider_slug: f5-networks
schema_file: json-schema/bigip-icontrol-rest-virtual-server-update-schema.json
slug: bigip-icontrol-rest-virtual-server-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VirtualServerUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a virtual server.\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"destination\": {\n      \"type\": \"string\"\n    },\n    \"ipProtocol\": {\n      \"type\": \"string\"\n    },\n    \"mask\": {\n      \"type\": \"string\"\n    },\n    \"pool\": {\n      \"type\": \"string\"\n    },\n    \"profiles\": {\n      \"type\": \"array\"\n    },\n    \"persist\": {\n      \"type\": \"array\"\n    },\n    \"source\": {\n      \"type\": \"string\"\n    },\n    \"sourcePort\": {\n      \"type\": \"string\"\n    },\n    \"translateAddress\": {\n      \"type\": \"string\"\n    },\n    \"translatePort\": {\n      \"type\": \"string\"\n    },\n    \"connectionLimit\": {\n      \"type\": \"integer\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"\
  disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"mirror\": {\n      \"type\": \"string\"\n    },\n    \"rateLimit\": {\n      \"type\": \"string\"\n    },\n    \"rules\": {\n      \"type\": \"array\"\n    },\n    \"vlans\": {\n      \"type\": \"array\"\n    },\n    \"vlansEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"vlansDisabled\": {\n      \"type\": \"boolean\"\n    },\n    \"fallbackPersistence\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/json-schema/bigip-icontrol-rest-virtual-server-update-schema.json
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
title: VirtualServerUpdate
---
