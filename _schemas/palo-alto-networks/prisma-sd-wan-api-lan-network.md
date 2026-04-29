---
description: LANNetwork schema from Palo Alto Networks Prisma SD-WAN API
layout: schema
name: LANNetwork
properties_list:
- description: Unique identifier for the LAN network.
  name: id
  type: string
- description: Name of the LAN network.
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Subnet CIDR for the LAN network (e.g., 192.168.1.0/24).
  name: network
  type: string
- description: VLAN identifier for this LAN network.
  name: vlan_id
  type: integer
- description: Whether the ION device serves DHCP for this network.
  name: dhcp_enabled
  type: boolean
- description: ''
  name: site_id
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-sd-wan-api-lan-network-schema.json
slug: prisma-sd-wan-api-lan-network
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LANNetwork\",\n  \"description\": \"LANNetwork schema from Palo Alto Networks Prisma SD-WAN API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-lan-network-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the LAN network.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the LAN network.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"network\": {\n      \"type\": \"string\",\n      \"description\": \"Subnet CIDR for the LAN network (e.g., 192.168.1.0/24).\"\n    },\n    \"vlan_id\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 4094,\n      \"description\": \"VLAN identifier for this\
  \ LAN network.\"\n    },\n    \"dhcp_enabled\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether the ION device serves DHCP for this network.\"\n    },\n    \"site_id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"network\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-lan-network-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: LANNetwork
---
