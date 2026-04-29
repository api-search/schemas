---
description: A gateway device managed by Aruba Central providing routing, VPN, and SD-WAN functionality.
layout: schema
name: Gateway
properties_list:
- description: Serial number of the gateway.
  name: serial
  type: string
- description: Name of the gateway.
  name: name
  type: string
- description: MAC address of the gateway.
  name: macaddr
  type: string
- description: Hardware model.
  name: model
  type: string
- description: Operational status.
  name: status
  type: string
- description: IP address of the gateway.
  name: ip_address
  type: string
- description: Firmware version.
  name: firmware_version
  type: string
- description: Configuration group.
  name: group_name
  type: string
- description: Site assignment.
  name: site
  type: string
- description: Uptime in seconds.
  name: uptime
  type: integer
- description: Number of connected clients.
  name: client_count
  type: integer
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-gateway-schema.json
slug: aruba-central-gateway
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Gateway\",\n  \"type\": \"object\",\n  \"description\": \"A gateway device managed by Aruba Central providing routing, VPN, and SD-WAN functionality.\",\n  \"properties\": {\n    \"serial\": {\n      \"type\": \"string\",\n      \"description\": \"Serial number of the gateway.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the gateway.\"\n    },\n    \"macaddr\": {\n      \"type\": \"string\",\n      \"description\": \"MAC address of the gateway.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware model.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Operational status.\"\n    },\n    \"ip_address\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the gateway.\"\n    },\n    \"firmware_version\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"Firmware version.\"\n    },\n    \"group_name\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration group.\"\n    },\n    \"site\": {\n      \"type\": \"string\",\n      \"description\": \"Site assignment.\"\n    },\n    \"uptime\": {\n      \"type\": \"integer\",\n      \"description\": \"Uptime in seconds.\"\n    },\n    \"client_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of connected clients.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-gateway-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: Gateway
---
