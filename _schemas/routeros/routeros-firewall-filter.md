---
description: Schema for RouterOS firewall packet filter rule
layout: schema
name: RouterOS Firewall Filter Rule
properties_list:
- description: Internal RouterOS record identifier
  name: .id
  type: string
- description: Firewall chain the rule belongs to
  name: chain
  type: string
- description: Action to take when rule matches
  name: action
  type: string
- description: Source IP address or CIDR range to match
  name: src-address
  type: string
- description: Destination IP address or CIDR range to match
  name: dst-address
  type: string
- description: Network protocol to match
  name: protocol
  type: string
- description: Source port or range
  name: src-port
  type: string
- description: Destination port or range
  name: dst-port
  type: string
- description: Incoming interface to match
  name: in-interface
  type: string
- description: Outgoing interface to match
  name: out-interface
  type: string
- description: Source must be in named address list
  name: src-address-list
  type: string
- description: Destination must be in named address list
  name: dst-address-list
  type: string
- description: Connection tracking state to match
  name: connection-state
  type: string
- description: ''
  name: disabled
  type: string
- description: ''
  name: comment
  type: string
provider_name: RouterOS
provider_slug: routeros
schema_file: json-schema/routeros-firewall-filter-schema.json
slug: routeros-firewall-filter
source_filename: routeros-firewall-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/routeros/main/json-schema/routeros-firewall-filter-schema.json\",\n  \"title\": \"RouterOS Firewall Filter Rule\",\n  \"description\": \"Schema for RouterOS firewall packet filter rule\",\n  \"type\": \"object\",\n  \"properties\": {\n    \".id\": {\n      \"type\": \"string\",\n      \"description\": \"Internal RouterOS record identifier\"\n    },\n    \"chain\": {\n      \"type\": \"string\",\n      \"description\": \"Firewall chain the rule belongs to\",\n      \"enum\": [\"input\", \"forward\", \"output\"],\n      \"examples\": [\"forward\"]\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"Action to take when rule matches\",\n      \"enum\": [\"accept\", \"drop\", \"reject\", \"log\", \"passthrough\", \"jump\", \"return\", \"tarpit\", \"fasttrack-connection\", \"add-src-to-address-list\", \"add-dst-to-address-list\"\
  ],\n      \"examples\": [\"accept\"]\n    },\n    \"src-address\": {\n      \"type\": \"string\",\n      \"description\": \"Source IP address or CIDR range to match\"\n    },\n    \"dst-address\": {\n      \"type\": \"string\",\n      \"description\": \"Destination IP address or CIDR range to match\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"description\": \"Network protocol to match\",\n      \"examples\": [\"tcp\", \"udp\", \"icmp\", \"gre\"]\n    },\n    \"src-port\": {\n      \"type\": \"string\",\n      \"description\": \"Source port or range\"\n    },\n    \"dst-port\": {\n      \"type\": \"string\",\n      \"description\": \"Destination port or range\"\n    },\n    \"in-interface\": {\n      \"type\": \"string\",\n      \"description\": \"Incoming interface to match\"\n    },\n    \"out-interface\": {\n      \"type\": \"string\",\n      \"description\": \"Outgoing interface to match\"\n    },\n    \"src-address-list\": {\n      \"type\": \"string\",\n  \
  \    \"description\": \"Source must be in named address list\"\n    },\n    \"dst-address-list\": {\n      \"type\": \"string\",\n      \"description\": \"Destination must be in named address list\"\n    },\n    \"connection-state\": {\n      \"type\": \"string\",\n      \"description\": \"Connection tracking state to match\",\n      \"examples\": [\"established\", \"related\", \"new\", \"invalid\"]\n    },\n    \"disabled\": {\n      \"type\": \"string\",\n      \"enum\": [\"true\", \"false\"]\n    },\n    \"comment\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\"chain\", \"action\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/json-schema/routeros-firewall-filter-schema.json
tags:
- Networking
- Routers
- Network Management
- Firewall
- MikroTik
title: RouterOS Firewall Filter Rule
---
