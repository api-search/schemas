---
description: An audit management log entry recording an administrative action.
layout: schema
name: AuditLog
properties_list:
- description: Action timestamp as Unix epoch milliseconds.
  name: timestamp
  type: integer
- description: ''
  name: actor_primary_username
  type: string
- description: ''
  name: actor_email
  type: string
- description: ''
  name: actor_type
  type: string
- description: Action subtype (e.g., Login, IpRangeModified, RuleUpdated).
  name: sub_type
  type: string
- description: ''
  name: result
  type: string
- description: ''
  name: reason
  type: string
- description: Source IP address of the action.
  name: ip
  type: string
- description: ''
  name: description
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xpanse-api-audit-log-schema.json
slug: cortex-xpanse-api-audit-log
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AuditLog\",\n  \"description\": \"An audit management log entry recording an administrative action.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xpanse-api-audit-log-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Action timestamp as Unix epoch milliseconds.\"\n    },\n    \"actor_primary_username\": {\n      \"type\": \"string\"\n    },\n    \"actor_email\": {\n      \"type\": \"string\"\n    },\n    \"actor_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"User\",\n        \"API\"\n      ]\n    },\n    \"sub_type\": {\n      \"type\": \"string\",\n      \"description\": \"Action subtype (e.g., Login, IpRangeModified, RuleUpdated).\"\n    },\n    \"result\": {\n      \"type\": \"string\",\n      \"enum\": [\n\
  \        \"SUCCESS\",\n        \"FAIL\"\n      ]\n    },\n    \"reason\": {\n      \"type\": \"string\"\n    },\n    \"ip\": {\n      \"type\": \"string\",\n      \"description\": \"Source IP address of the action.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xpanse-api-audit-log-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AuditLog
---
