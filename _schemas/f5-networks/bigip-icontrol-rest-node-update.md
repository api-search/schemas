---
description: Request body for updating a node.
layout: schema
name: NodeUpdate
properties_list:
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
- description: ''
  name: logging
  type: string
provider_name: F5 Networks
provider_slug: f5-networks
schema_file: json-schema/bigip-icontrol-rest-node-update-schema.json
slug: bigip-icontrol-rest-node-update
source_filename: bigip-icontrol-rest-node-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NodeUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a node.\",\n  \"properties\": {\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"connectionLimit\": {\n      \"type\": \"integer\"\n    },\n    \"monitor\": {\n      \"type\": \"string\"\n    },\n    \"rateLimit\": {\n      \"type\": \"string\"\n    },\n    \"ratio\": {\n      \"type\": \"integer\"\n    },\n    \"session\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"logging\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/json-schema/bigip-icontrol-rest-node-update-schema.json
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
title: NodeUpdate
---
