---
description: Request body for adding a new pool member.
layout: schema
name: PoolMemberCreate
properties_list:
- description: Member name in address:port format. If a node with the address does not exist, one will be created.
  name: name
  type: string
- description: IP address if it differs from the name.
  name: address
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: connectionLimit
  type: integer
- description: ''
  name: monitor
  type: string
- description: ''
  name: priorityGroup
  type: integer
- description: ''
  name: rateLimit
  type: string
- description: ''
  name: ratio
  type: integer
- description: ''
  name: session
  type: string
- description: ''
  name: state
  type: string
provider_name: F5 Networks
provider_slug: f5-networks
schema_file: json-schema/bigip-icontrol-rest-pool-member-create-schema.json
slug: bigip-icontrol-rest-pool-member-create
source_filename: bigip-icontrol-rest-pool-member-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PoolMemberCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for adding a new pool member.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Member name in address:port format. If a node with the address does not exist, one will be created.\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"IP address if it differs from the name.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"connectionLimit\": {\n      \"type\": \"integer\"\n    },\n    \"monitor\": {\n      \"type\": \"string\"\n    },\n    \"priorityGroup\": {\n      \"type\": \"integer\"\n    },\n    \"rateLimit\": {\n      \"type\": \"string\"\n    },\n    \"ratio\": {\n      \"type\": \"integer\"\n    },\n    \"session\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n  \
  \  }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/json-schema/bigip-icontrol-rest-pool-member-create-schema.json
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
title: PoolMemberCreate
---
