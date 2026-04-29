---
description: ''
layout: schema
name: Check Point Access Rule
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: layer
  type: string
- description: ''
  name: uid
  type: string
- description: ''
  name: source
  type: array
- description: ''
  name: destination
  type: array
- description: ''
  name: service
  type: array
- description: ''
  name: action
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: track
  type: string
provider_name: Check Point
provider_slug: checkpoint
schema_file: json-schema/checkpoint-access-rule-schema.json
slug: checkpoint-access-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.checkpoint.com/schemas/access-rule.json\",\n  \"title\": \"Check Point Access Rule\",\n  \"type\": \"object\",\n  \"required\": [\"layer\"],\n  \"properties\": {\n    \"name\": { \"type\": \"string\" },\n    \"layer\": { \"type\": \"string\" },\n    \"uid\": { \"type\": \"string\" },\n    \"source\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"destination\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"service\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\"Accept\", \"Drop\", \"Reject\", \"Inline Layer\"]\n    },\n    \"enabled\": { \"type\": \"boolean\" },\n    \"track\": { \"type\": \"string\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/checkpoint/refs/heads/main/json-schema/checkpoint-access-rule-schema.json
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
title: Check Point Access Rule
---
