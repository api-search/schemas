---
description: Schema for RouterOS IP address configuration resource
layout: schema
name: RouterOS IP Address
properties_list:
- description: Internal RouterOS record identifier (asterisk-prefixed integer)
  name: .id
  type: string
- description: IP address with prefix length in CIDR notation
  name: address
  type: string
- description: Network address derived from address and mask
  name: network
  type: string
- description: Network interface the address is assigned to
  name: interface
  type: string
- description: Whether the address was dynamically assigned (RouterOS returns booleans as strings)
  name: dynamic
  type: string
- description: Whether the address is administratively disabled
  name: disabled
  type: string
- description: Optional administrator comment
  name: comment
  type: string
provider_name: RouterOS
provider_slug: routeros
schema_file: json-schema/routeros-ip-address-schema.json
slug: routeros-ip-address
source_filename: routeros-ip-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/routeros/main/json-schema/routeros-ip-address-schema.json\",\n  \"title\": \"RouterOS IP Address\",\n  \"description\": \"Schema for RouterOS IP address configuration resource\",\n  \"type\": \"object\",\n  \"properties\": {\n    \".id\": {\n      \"type\": \"string\",\n      \"description\": \"Internal RouterOS record identifier (asterisk-prefixed integer)\",\n      \"pattern\": \"^\\\\*[0-9]+$\",\n      \"examples\": [\"*1\", \"*2\"]\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"IP address with prefix length in CIDR notation\",\n      \"pattern\": \"^\\\\d{1,3}\\\\.\\\\d{1,3}\\\\.\\\\d{1,3}\\\\.\\\\d{1,3}/\\\\d{1,2}$\",\n      \"examples\": [\"192.168.1.1/24\", \"10.0.0.1/8\"]\n    },\n    \"network\": {\n      \"type\": \"string\",\n      \"description\": \"Network address derived from address and mask\",\n\
  \      \"examples\": [\"192.168.1.0\", \"10.0.0.0\"]\n    },\n    \"interface\": {\n      \"type\": \"string\",\n      \"description\": \"Network interface the address is assigned to\",\n      \"examples\": [\"ether1\", \"bridge1\", \"wlan1\"]\n    },\n    \"dynamic\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the address was dynamically assigned (RouterOS returns booleans as strings)\",\n      \"enum\": [\"true\", \"false\"]\n    },\n    \"disabled\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the address is administratively disabled\",\n      \"enum\": [\"true\", \"false\"]\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Optional administrator comment\"\n    }\n  },\n  \"required\": [\"address\", \"interface\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/json-schema/routeros-ip-address-schema.json
tags:
- Networking
- Routers
- Network Management
- Firewall
- MikroTik
title: RouterOS IP Address
---
