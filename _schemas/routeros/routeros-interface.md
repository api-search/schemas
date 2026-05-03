---
description: Schema for RouterOS network interface resource
layout: schema
name: RouterOS Interface
properties_list:
- description: Internal RouterOS record identifier
  name: .id
  type: string
- description: Interface name
  name: name
  type: string
- description: Interface type
  name: type
  type: string
- description: Maximum Transmission Unit in bytes
  name: mtu
  type: string
- description: Hardware MAC address
  name: mac-address
  type: string
- description: Whether the interface is currently active
  name: running
  type: string
- description: Whether the interface is administratively disabled
  name: disabled
  type: string
- description: Optional administrator comment
  name: comment
  type: string
provider_name: RouterOS
provider_slug: routeros
schema_file: json-schema/routeros-interface-schema.json
slug: routeros-interface
source_filename: routeros-interface-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/routeros/main/json-schema/routeros-interface-schema.json\",\n  \"title\": \"RouterOS Interface\",\n  \"description\": \"Schema for RouterOS network interface resource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \".id\": {\n      \"type\": \"string\",\n      \"description\": \"Internal RouterOS record identifier\",\n      \"examples\": [\"*1\"]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Interface name\",\n      \"examples\": [\"ether1\", \"wlan1\", \"bridge1\", \"vlan100\"]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Interface type\",\n      \"examples\": [\"ether\", \"bridge\", \"vlan\", \"pppoe\", \"wireless\", \"loopback\", \"veth\"]\n    },\n    \"mtu\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum Transmission Unit in bytes\",\n      \"examples\"\
  : [\"1500\", \"9000\"]\n    },\n    \"mac-address\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware MAC address\",\n      \"pattern\": \"^([0-9A-Fa-f]{2}:){5}[0-9A-Fa-f]{2}$\",\n      \"examples\": [\"AA:BB:CC:DD:EE:FF\"]\n    },\n    \"running\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the interface is currently active\",\n      \"enum\": [\"true\", \"false\"]\n    },\n    \"disabled\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the interface is administratively disabled\",\n      \"enum\": [\"true\", \"false\"]\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Optional administrator comment\"\n    }\n  },\n  \"required\": [\"name\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/json-schema/routeros-interface-schema.json
tags:
- Networking
- Routers
- Network Management
- Firewall
- MikroTik
title: RouterOS Interface
---
