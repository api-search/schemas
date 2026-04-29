---
description: An endpoint enrolled in XSIAM protection.
layout: schema
name: Endpoint
properties_list:
- description: ''
  name: endpoint_id
  type: string
- description: ''
  name: endpoint_name
  type: string
- description: ''
  name: endpoint_type
  type: string
- description: ''
  name: endpoint_status
  type: string
- description: ''
  name: os_type
  type: string
- description: ''
  name: ip
  type: array
- description: ''
  name: users
  type: array
- description: ''
  name: domain
  type: string
- description: ''
  name: first_seen
  type: integer
- description: ''
  name: last_seen
  type: integer
- description: ''
  name: endpoint_version
  type: string
- description: ''
  name: content_version
  type: string
- description: ''
  name: is_isolated
  type: string
- description: ''
  name: scan_status
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsiam-api-endpoint-schema.json
slug: cortex-xsiam-api-endpoint
source_filename: cortex-xsiam-api-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Endpoint\",\n  \"description\": \"An endpoint enrolled in XSIAM protection.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsiam-api-endpoint-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endpoint_id\": {\n      \"type\": \"string\"\n    },\n    \"endpoint_name\": {\n      \"type\": \"string\"\n    },\n    \"endpoint_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SERVER\",\n        \"WORKSTATION\",\n        \"LAPTOP\"\n      ]\n    },\n    \"endpoint_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CONNECTED\",\n        \"DISCONNECTED\",\n        \"LOST\",\n        \"UNINSTALLED\"\n      ]\n    },\n    \"os_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AGENT_OS_WINDOWS\",\n        \"AGENT_OS_LINUX\",\n        \"AGENT_OS_MAC\"\n    \
  \  ]\n    },\n    \"ip\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"users\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"domain\": {\n      \"type\": \"string\"\n    },\n    \"first_seen\": {\n      \"type\": \"integer\"\n    },\n    \"last_seen\": {\n      \"type\": \"integer\"\n    },\n    \"endpoint_version\": {\n      \"type\": \"string\"\n    },\n    \"content_version\": {\n      \"type\": \"string\"\n    },\n    \"is_isolated\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AGENT_ISOLATED\",\n        \"AGENT_UNISOLATED\",\n        \"PENDING_ISOLATION\",\n        \"PENDING_UNISOLATION\"\n      ]\n    },\n    \"scan_status\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsiam-api-endpoint-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Endpoint
---
