---
description: A wireless SSID or wired network managed by Central.
layout: schema
name: Network
properties_list:
- description: Extended Service Set Identifier (network name).
  name: essid
  type: string
- description: Network type.
  name: type
  type: string
- description: Number of connected clients.
  name: client_count
  type: integer
- description: Configuration group the network belongs to.
  name: group_name
  type: string
- description: Site assignment.
  name: site
  type: string
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-network-schema.json
slug: aruba-central-network
source_filename: aruba-central-network-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Network\",\n  \"type\": \"object\",\n  \"description\": \"A wireless SSID or wired network managed by Central.\",\n  \"properties\": {\n    \"essid\": {\n      \"type\": \"string\",\n      \"description\": \"Extended Service Set Identifier (network name).\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Network type.\"\n    },\n    \"client_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of connected clients.\"\n    },\n    \"group_name\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration group the network belongs to.\"\n    },\n    \"site\": {\n      \"type\": \"string\",\n      \"description\": \"Site assignment.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-network-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: Network
---
