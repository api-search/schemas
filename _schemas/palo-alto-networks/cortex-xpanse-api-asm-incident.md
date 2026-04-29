---
description: An attack surface incident representing a confirmed exposure requiring remediation.
layout: schema
name: AsmIncident
properties_list:
- description: Unique attack surface incident identifier.
  name: incident_id
  type: string
- description: ''
  name: incident_name
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: severity
  type: string
- description: Attack surface rule types that triggered this incident.
  name: incident_type
  type: array
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
  name: description
  type: string
- description: Incident creation timestamp as Unix epoch milliseconds.
  name: creation_time
  type: integer
- description: ''
  name: modification_time
  type: integer
- description: ''
  name: resolved_by
  type: string
- description: ''
  name: resolve_comment
  type: string
- description: ''
  name: tags
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xpanse-api-asm-incident-schema.json
slug: cortex-xpanse-api-asm-incident
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AsmIncident\",\n  \"description\": \"An attack surface incident representing a confirmed exposure requiring remediation.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xpanse-api-asm-incident-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"incident_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique attack surface incident identifier.\"\n    },\n    \"incident_name\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"new\",\n        \"under_investigation\",\n        \"resolved\",\n        \"resolved_no_risk\",\n        \"resolved_risk_accepted\",\n        \"resolved_contested_asset\",\n        \"resolved_remediated_automatically\"\n      ]\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n\
  \        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\",\n        \"informational\"\n      ]\n    },\n    \"incident_type\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Attack surface rule types that triggered this incident.\"\n    },\n    \"assigned_user_mail\": {\n      \"type\": \"string\"\n    },\n    \"assigned_user_pretty_name\": {\n      \"type\": \"string\"\n    },\n    \"alert_count\": {\n      \"type\": \"integer\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"creation_time\": {\n      \"type\": \"integer\",\n      \"description\": \"Incident creation timestamp as Unix epoch milliseconds.\"\n    },\n    \"modification_time\": {\n      \"type\": \"integer\"\n    },\n    \"resolved_by\": {\n      \"type\": \"string\"\n    },\n    \"resolve_comment\": {\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n \
  \       \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\"\n          },\n          \"value\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xpanse-api-asm-incident-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AsmIncident
---
