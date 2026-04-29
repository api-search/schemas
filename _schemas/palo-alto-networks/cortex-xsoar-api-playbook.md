---
description: A Cortex XSOAR playbook defining an automated response workflow.
layout: schema
name: Playbook
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: version
  type: integer
- description: ''
  name: description
  type: string
- description: ''
  name: tags
  type: array
- description: Minimum XSOAR version required.
  name: fromVersion
  type: string
- description: ''
  name: toVersion
  type: string
- description: ''
  name: deprecated
  type: boolean
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsoar-api-playbook-schema.json
slug: cortex-xsoar-api-playbook
source_filename: cortex-xsoar-api-playbook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Playbook\",\n  \"description\": \"A Cortex XSOAR playbook defining an automated response workflow.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-playbook-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"integer\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"fromVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Minimum XSOAR version required.\"\n    },\n    \"toVersion\": {\n      \"type\": \"string\"\n    },\n    \"deprecated\": {\n      \"type\": \"boolean\"\n    }\n  }\n\
  }\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsoar-api-playbook-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Playbook
---
