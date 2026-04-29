---
description: ''
layout: schema
name: Check Point Host Object
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: ip-address
  type: string
- description: ''
  name: ipv4-address
  type: string
- description: ''
  name: ipv6-address
  type: string
- description: ''
  name: comments
  type: string
- description: ''
  name: color
  type: string
- description: ''
  name: uid
  type: string
provider_name: Check Point
provider_slug: checkpoint
schema_file: json-schema/checkpoint-host-schema.json
slug: checkpoint-host
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.checkpoint.com/schemas/host.json\",\n  \"title\": \"Check Point Host Object\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"ip-address\"],\n  \"properties\": {\n    \"name\": { \"type\": \"string\" },\n    \"ip-address\": { \"type\": \"string\" },\n    \"ipv4-address\": { \"type\": \"string\" },\n    \"ipv6-address\": { \"type\": \"string\" },\n    \"comments\": { \"type\": \"string\" },\n    \"color\": { \"type\": \"string\" },\n    \"uid\": { \"type\": \"string\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/json-schema/checkpoint-host-schema.json
tags:
- Cloud Security
- Cybersecurity
- Endpoint Security
- Firewall
- Identity Awareness
- Mobile Security
- Network Security
- Security
- Threat Prevention
- WAF
title: Check Point Host Object
---
