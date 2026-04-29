---
description: A Cortex XDR alert representing a single detection event.
layout: schema
name: Alert
properties_list:
- description: ''
  name: alert_id
  type: string
- description: Detection timestamp as Unix epoch milliseconds.
  name: detection_timestamp
  type: integer
- description: Alert name or rule name that triggered this alert.
  name: name
  type: string
- description: Alert category (e.g., Malware, Exploit, Lateral Movement).
  name: category
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: host_ip
  type: array
- description: ''
  name: host_name
  type: string
- description: ''
  name: user_name
  type: string
- description: ''
  name: mac
  type: array
- description: Data source that generated the alert.
  name: source
  type: string
- description: Action taken on the alert.
  name: action
  type: string
- description: ''
  name: action_pretty
  type: string
- description: ''
  name: severity
  type: string
- description: ''
  name: matching_status
  type: string
- description: ''
  name: alert_type
  type: string
- description: ''
  name: resolution_status
  type: string
- description: ''
  name: resolution_comment
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xdr-api-alert-schema.json
slug: cortex-xdr-api-alert
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Alert\",\n  \"description\": \"A Cortex XDR alert representing a single detection event.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xdr-api-alert-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alert_id\": {\n      \"type\": \"string\"\n    },\n    \"detection_timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Detection timestamp as Unix epoch milliseconds.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Alert name or rule name that triggered this alert.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Alert category (e.g., Malware, Exploit, Lateral Movement).\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"host_ip\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"\
  type\": \"string\"\n      }\n    },\n    \"host_name\": {\n      \"type\": \"string\"\n    },\n    \"user_name\": {\n      \"type\": \"string\"\n    },\n    \"mac\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Data source that generated the alert.\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"Action taken on the alert.\"\n    },\n    \"action_pretty\": {\n      \"type\": \"string\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\",\n        \"informational\",\n        \"unknown\"\n      ]\n    },\n    \"matching_status\": {\n      \"type\": \"string\"\n    },\n    \"alert_type\": {\n      \"type\": \"string\"\n    },\n    \"resolution_status\": {\n      \"type\": \"string\"\n    },\n    \"resolution_comment\": {\n    \
  \  \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xdr-api-alert-schema.json
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
