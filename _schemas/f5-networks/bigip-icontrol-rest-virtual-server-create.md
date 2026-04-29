---
description: Request body for creating a new virtual server.
layout: schema
name: VirtualServerCreate
properties_list:
- description: Name of the virtual server.
  name: name
  type: string
- description: Administrative partition.
  name: partition
  type: string
- description: Destination address and port in /partition/address:port format.
  name: destination
  type: string
- description: User-defined description.
  name: description
  type: string
- description: IP protocol.
  name: ipProtocol
  type: string
- description: Destination network mask.
  name: mask
  type: string
- description: Default pool full path.
  name: pool
  type: string
- description: Profiles to apply.
  name: profiles
  type: array
- description: Persistence profiles to apply.
  name: persist
  type: array
- description: Source address filter.
  name: source
  type: string
- description: Source port translation behavior.
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
provider_name: F5 Networks
provider_slug: f5-networks
schema_file: json-schema/bigip-icontrol-rest-virtual-server-create-schema.json
slug: bigip-icontrol-rest-virtual-server-create
source_filename: bigip-icontrol-rest-virtual-server-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VirtualServerCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new virtual server.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the virtual server.\"\n    },\n    \"partition\": {\n      \"type\": \"string\",\n      \"description\": \"Administrative partition.\"\n    },\n    \"destination\": {\n      \"type\": \"string\",\n      \"description\": \"Destination address and port in /partition/address:port format.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"User-defined description.\"\n    },\n    \"ipProtocol\": {\n      \"type\": \"string\",\n      \"description\": \"IP protocol.\"\n    },\n    \"mask\": {\n      \"type\": \"string\",\n      \"description\": \"Destination network mask.\"\n    },\n    \"pool\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Default pool full path.\"\n    },\n    \"profiles\": {\n      \"type\": \"array\",\n      \"description\": \"Profiles to apply.\"\n    },\n    \"persist\": {\n      \"type\": \"array\",\n      \"description\": \"Persistence profiles to apply.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source address filter.\"\n    },\n    \"sourcePort\": {\n      \"type\": \"string\",\n      \"description\": \"Source port translation behavior.\"\n    },\n    \"translateAddress\": {\n      \"type\": \"string\"\n    },\n    \"translatePort\": {\n      \"type\": \"string\"\n    },\n    \"connectionLimit\": {\n      \"type\": \"integer\"\n    },\n    \"rules\": {\n      \"type\": \"array\"\n    },\n    \"vlans\": {\n      \"type\": \"array\"\n    },\n    \"vlansEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"vlansDisabled\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/json-schema/bigip-icontrol-rest-virtual-server-create-schema.json
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
title: VirtualServerCreate
---
