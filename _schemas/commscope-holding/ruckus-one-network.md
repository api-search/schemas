---
description: Schema for a Wi-Fi network resource in the RUCKUS One API.
layout: schema
name: RUCKUS One Network
properties_list:
- description: RUCKUS One-assigned network UID.
  name: id
  type: string
- description: Display name for the network.
  name: name
  type: string
- description: Service set identifier broadcast by APs.
  name: ssid
  type: string
- description: Security mode for the network.
  name: security
  type: string
- description: UID of the venue this network belongs to.
  name: venueId
  type: string
- description: Optional VLAN tag.
  name: vlanId
  type: integer
provider_name: CommScope Holding
provider_slug: commscope-holding
schema_file: json-schema/ruckus-one-network-schema.json
slug: ruckus-one-network
source_filename: ruckus-one-network-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/commscope-holding/refs/heads/main/json-schema/ruckus-one-network-schema.json\",\n  \"title\": \"RUCKUS One Network\",\n  \"description\": \"Schema for a Wi-Fi network resource in the RUCKUS One API.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"ssid\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"RUCKUS One-assigned network UID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the network.\"\n    },\n    \"ssid\": {\n      \"type\": \"string\",\n      \"description\": \"Service set identifier broadcast by APs.\"\n    },\n    \"security\": {\n      \"type\": \"string\",\n      \"enum\": [\"open\", \"wpa2\", \"wpa3\", \"wpa2wpa3\", \"dpsk\"],\n      \"description\": \"Security mode for the network.\"\n    },\n \
  \   \"venueId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"UID of the venue this network belongs to.\"\n    },\n    \"vlanId\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 4094,\n      \"description\": \"Optional VLAN tag.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/commscope-holding/refs/heads/main/json-schema/ruckus-one-network-schema.json
tags:
- Access Points
- Cabling
- Connectivity
- ICX Switches
- Infrastructure
- Networking
- RUCKUS
- Wi-Fi
title: RUCKUS One Network
---
