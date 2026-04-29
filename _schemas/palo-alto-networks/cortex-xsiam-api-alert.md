---
description: A XSIAM alert representing a detection from any ingested data source.
layout: schema
name: Alert
properties_list:
- description: ''
  name: alert_id
  type: string
- description: ''
  name: detection_timestamp
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: category
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: severity
  type: string
- description: Data source that generated this alert.
  name: source
  type: string
- description: ''
  name: host_name
  type: string
- description: ''
  name: user_name
  type: string
- description: ''
  name: action
  type: string
- description: ''
  name: alert_type
  type: string
- description: ''
  name: resolution_status
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsiam-api-alert-schema.json
slug: cortex-xsiam-api-alert
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Alert\",\n  \"description\": \"A XSIAM alert representing a detection from any ingested data source.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsiam-api-alert-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alert_id\": {\n      \"type\": \"string\"\n    },\n    \"detection_timestamp\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"category\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\",\n        \"informational\",\n        \"unknown\"\n      ]\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Data source that generated\
  \ this alert.\"\n    },\n    \"host_name\": {\n      \"type\": \"string\"\n    },\n    \"user_name\": {\n      \"type\": \"string\"\n    },\n    \"action\": {\n      \"type\": \"string\"\n    },\n    \"alert_type\": {\n      \"type\": \"string\"\n    },\n    \"resolution_status\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsiam-api-alert-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Alert
---
