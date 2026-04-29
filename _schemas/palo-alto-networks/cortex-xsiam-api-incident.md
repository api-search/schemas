---
description: A XSIAM incident correlating related alerts into a unified investigation.
layout: schema
name: Incident
properties_list:
- description: ''
  name: incident_id
  type: string
- description: ''
  name: incident_name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: severity
  type: string
- description: ''
  name: assigned_user_mail
  type: string
- description: ''
  name: assigned_user_pretty_name
  type: string
- description: ''
  name: alert_count
  type: integer
- description: Creation timestamp as Unix epoch milliseconds.
  name: creation_time
  type: integer
- description: ''
  name: modification_time
  type: integer
- description: ''
  name: detection_time
  type: integer
- description: ''
  name: starred
  type: boolean
- description: ''
  name: xdr_url
  type: string
- description: ''
  name: mitre_tactics_ids_and_names
  type: array
- description: ''
  name: mitre_techniques_ids_and_names
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsiam-api-incident-schema.json
slug: cortex-xsiam-api-incident
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Incident\",\n  \"description\": \"A XSIAM incident correlating related alerts into a unified investigation.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsiam-api-incident-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"incident_id\": {\n      \"type\": \"string\"\n    },\n    \"incident_name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"new\",\n        \"under_investigation\",\n        \"resolved_threat_handled\",\n        \"resolved_known_issue\",\n        \"resolved_duplicate\",\n        \"resolved_false_positive\",\n        \"resolved_other\"\n      ]\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\"\
  ,\n        \"medium\",\n        \"low\",\n        \"informational\",\n        \"unknown\"\n      ]\n    },\n    \"assigned_user_mail\": {\n      \"type\": \"string\"\n    },\n    \"assigned_user_pretty_name\": {\n      \"type\": \"string\"\n    },\n    \"alert_count\": {\n      \"type\": \"integer\"\n    },\n    \"creation_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Creation timestamp as Unix epoch milliseconds.\"\n    },\n    \"modification_time\": {\n      \"type\": \"integer\"\n    },\n    \"detection_time\": {\n      \"type\": \"integer\"\n    },\n    \"starred\": {\n      \"type\": \"boolean\"\n    },\n    \"xdr_url\": {\n      \"type\": \"string\"\n    },\n    \"mitre_tactics_ids_and_names\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"mitre_techniques_ids_and_names\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsiam-api-incident-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Incident
---
