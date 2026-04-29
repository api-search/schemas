---
description: A Cortex XDR incident grouping related alerts.
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
- description: ''
  name: low_severity_alert_count
  type: integer
- description: ''
  name: med_severity_alert_count
  type: integer
- description: ''
  name: high_severity_alert_count
  type: integer
- description: ''
  name: critical_severity_alert_count
  type: integer
- description: ''
  name: user_count
  type: integer
- description: ''
  name: host_count
  type: integer
- description: Incident creation timestamp as Unix epoch milliseconds.
  name: creation_time
  type: integer
- description: Last modification timestamp as Unix epoch milliseconds.
  name: modification_time
  type: integer
- description: ''
  name: detection_time
  type: integer
- description: ''
  name: starred
  type: boolean
- description: Direct URL to the incident in the XDR console.
  name: xdr_url
  type: string
- description: ''
  name: rule_based_score
  type: integer
- description: ''
  name: manual_score
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xdr-api-incident-schema.json
slug: cortex-xdr-api-incident
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Incident\",\n  \"description\": \"A Cortex XDR incident grouping related alerts.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xdr-api-incident-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"incident_id\": {\n      \"type\": \"string\"\n    },\n    \"incident_name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"new\",\n        \"under_investigation\",\n        \"resolved_threat_handled\",\n        \"resolved_known_issue\",\n        \"resolved_duplicate\",\n        \"resolved_false_positive\",\n        \"resolved_other\"\n      ]\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n \
  \       \"low\",\n        \"informational\",\n        \"unknown\"\n      ]\n    },\n    \"assigned_user_mail\": {\n      \"type\": \"string\"\n    },\n    \"assigned_user_pretty_name\": {\n      \"type\": \"string\"\n    },\n    \"alert_count\": {\n      \"type\": \"integer\"\n    },\n    \"low_severity_alert_count\": {\n      \"type\": \"integer\"\n    },\n    \"med_severity_alert_count\": {\n      \"type\": \"integer\"\n    },\n    \"high_severity_alert_count\": {\n      \"type\": \"integer\"\n    },\n    \"critical_severity_alert_count\": {\n      \"type\": \"integer\"\n    },\n    \"user_count\": {\n      \"type\": \"integer\"\n    },\n    \"host_count\": {\n      \"type\": \"integer\"\n    },\n    \"creation_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Incident creation timestamp as Unix epoch milliseconds.\"\n    },\n    \"modification_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Last modification timestamp as Unix epoch milliseconds.\"\n\
  \    },\n    \"detection_time\": {\n      \"type\": \"integer\"\n    },\n    \"starred\": {\n      \"type\": \"boolean\"\n    },\n    \"xdr_url\": {\n      \"type\": \"string\",\n      \"description\": \"Direct URL to the incident in the XDR console.\"\n    },\n    \"rule_based_score\": {\n      \"type\": \"integer\"\n    },\n    \"manual_score\": {\n      \"type\": \"integer\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xdr-api-incident-schema.json
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
