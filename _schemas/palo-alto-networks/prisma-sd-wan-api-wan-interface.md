---
description: WANInterface schema from Palo Alto Networks Prisma SD-WAN API
layout: schema
name: WANInterface
properties_list:
- description: Unique identifier for the WAN interface.
  name: id
  type: string
- description: Name of the WAN interface.
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Type of WAN connection.
  name: type
  type: string
- description: Downstream bandwidth in Mbps.
  name: link_bw_down
  type: number
- description: Upstream bandwidth in Mbps.
  name: link_bw_up
  type: number
- description: Cost metric for path selection. Lower cost is preferred.
  name: cost
  type: integer
- description: Whether Link Quality Monitoring is enabled.
  name: lqm_enabled
  type: boolean
- description: WAN interface label for policy-based routing.
  name: label_id
  type: string
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
schema_file: json-schema/prisma-sd-wan-api-wan-interface-schema.json
slug: prisma-sd-wan-api-wan-interface
source_filename: prisma-sd-wan-api-wan-interface-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WANInterface\",\n  \"description\": \"WANInterface schema from Palo Alto Networks Prisma SD-WAN API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-wan-interface-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the WAN interface.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the WAN interface.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"publicwan\",\n        \"privatewan\"\n      ],\n      \"description\": \"Type of WAN connection.\"\n    },\n    \"link_bw_down\": {\n      \"type\": \"number\",\n      \"description\": \"Downstream bandwidth\
  \ in Mbps.\"\n    },\n    \"link_bw_up\": {\n      \"type\": \"number\",\n      \"description\": \"Upstream bandwidth in Mbps.\"\n    },\n    \"cost\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 255,\n      \"description\": \"Cost metric for path selection. Lower cost is preferred.\"\n    },\n    \"lqm_enabled\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Whether Link Quality Monitoring is enabled.\"\n    },\n    \"label_id\": {\n      \"type\": \"string\",\n      \"description\": \"WAN interface label for policy-based routing.\"\n    },\n    \"site_id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\"\n  ]\n\
  }\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-wan-interface-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: WANInterface
---
