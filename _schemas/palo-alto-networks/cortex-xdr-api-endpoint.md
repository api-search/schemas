---
description: An endpoint enrolled in Cortex XDR protection.
layout: schema
name: Endpoint
properties_list:
- description: Unique endpoint identifier.
  name: endpoint_id
  type: string
- description: Endpoint hostname.
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
- description: IP addresses assigned to the endpoint.
  name: ip
  type: array
- description: Users logged into the endpoint.
  name: users
  type: array
- description: ''
  name: domain
  type: string
- description: ''
  name: alias
  type: string
- description: First connection timestamp as Unix epoch milliseconds.
  name: first_seen
  type: integer
- description: Last connection timestamp as Unix epoch milliseconds.
  name: last_seen
  type: integer
- description: Cortex XDR agent content version.
  name: content_version
  type: string
- description: ''
  name: installation_package
  type: string
- description: ''
  name: active_directory
  type: string
- description: ''
  name: install_date
  type: integer
- description: Cortex XDR agent version.
  name: endpoint_version
  type: string
- description: ''
  name: is_isolated
  type: string
- description: ''
  name: isolation_reason
  type: string
- description: ''
  name: scan_status
  type: string
- description: ''
  name: group_name
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xdr-api-endpoint-schema.json
slug: cortex-xdr-api-endpoint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Endpoint\",\n  \"description\": \"An endpoint enrolled in Cortex XDR protection.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xdr-api-endpoint-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endpoint_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique endpoint identifier.\"\n    },\n    \"endpoint_name\": {\n      \"type\": \"string\",\n      \"description\": \"Endpoint hostname.\"\n    },\n    \"endpoint_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SERVER\",\n        \"WORKSTATION\",\n        \"LAPTOP\"\n      ]\n    },\n    \"endpoint_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CONNECTED\",\n        \"DISCONNECTED\",\n        \"LOST\",\n        \"UNINSTALLED\"\n      ]\n    },\n    \"os_type\": {\n      \"type\": \"string\",\n \
  \     \"enum\": [\n        \"AGENT_OS_WINDOWS\",\n        \"AGENT_OS_LINUX\",\n        \"AGENT_OS_MAC\"\n      ]\n    },\n    \"ip\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"IP addresses assigned to the endpoint.\"\n    },\n    \"users\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Users logged into the endpoint.\"\n    },\n    \"domain\": {\n      \"type\": \"string\"\n    },\n    \"alias\": {\n      \"type\": \"string\"\n    },\n    \"first_seen\": {\n      \"type\": \"integer\",\n      \"description\": \"First connection timestamp as Unix epoch milliseconds.\"\n    },\n    \"last_seen\": {\n      \"type\": \"integer\",\n      \"description\": \"Last connection timestamp as Unix epoch milliseconds.\"\n    },\n    \"content_version\": {\n      \"type\": \"string\",\n      \"description\": \"Cortex XDR agent content version.\"\n    },\n   \
  \ \"installation_package\": {\n      \"type\": \"string\"\n    },\n    \"active_directory\": {\n      \"type\": \"string\"\n    },\n    \"install_date\": {\n      \"type\": \"integer\"\n    },\n    \"endpoint_version\": {\n      \"type\": \"string\",\n      \"description\": \"Cortex XDR agent version.\"\n    },\n    \"is_isolated\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AGENT_ISOLATED\",\n        \"AGENT_UNISOLATED\",\n        \"PENDING_ISOLATION\",\n        \"PENDING_UNISOLATION\"\n      ]\n    },\n    \"isolation_reason\": {\n      \"type\": \"string\"\n    },\n    \"scan_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SCAN_STATUS_NONE\",\n        \"SCAN_STATUS_PENDING\",\n        \"SCAN_STATUS_IN_PROGRESS\",\n        \"SCAN_STATUS_DONE\",\n        \"SCAN_STATUS_FAILED\",\n        \"SCAN_STATUS_CANCELLED\"\n      ]\n    },\n    \"group_name\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n\
  \  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xdr-api-endpoint-schema.json
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
