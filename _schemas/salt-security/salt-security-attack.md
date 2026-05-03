---
description: An API attack event detected and analyzed by the Salt Security threat protection engine.
layout: schema
name: Salt Security API Attack
properties_list:
- description: Unique identifier for the attack event
  name: id
  type: string
- description: Type of API attack detected
  name: attack_type
  type: string
- description: Severity level of the attack
  name: severity
  type: string
- description: Current status of the attack
  name: status
  type: string
- description: Source IP address of the attacker
  name: source_ip
  type: string
- description: API endpoint being attacked
  name: target_endpoint
  type: string
- description: ID of the API being attacked
  name: target_api_id
  type: string
- description: Pattern or signature that identified this as an attack
  name: attack_signature
  type: string
- description: Number of malicious requests in this attack
  name: request_count
  type: integer
- description: User IDs or identifiers affected by this attack
  name: affected_users
  type: array
- description: Whether sensitive data was potentially exposed
  name: data_exposed
  type: boolean
- description: ''
  name: mitigation_actions
  type: array
- description: ''
  name: remediation
  type: object
- description: Timestamp when attack was first detected
  name: detected_at
  type: string
- description: Timestamp when attack was resolved
  name: resolved_at
  type: string
provider_name: Salt Security
provider_slug: salt-security
schema_file: json-schema/salt-security-attack-schema.json
slug: salt-security-attack
source_filename: salt-security-attack-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/salt-security/json-schema/salt-security-attack-schema.json\",\n  \"title\": \"Salt Security API Attack\",\n  \"description\": \"An API attack event detected and analyzed by the Salt Security threat protection engine.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the attack event\"\n    },\n    \"attack_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of API attack detected\",\n      \"enum\": [\n        \"BOLA\",\n        \"BFLA\",\n        \"Injection\",\n        \"Authentication Bypass\",\n        \"Credential Stuffing\",\n        \"Account Takeover\",\n        \"Excessive Data Exposure\",\n        \"Mass Assignment\",\n        \"Rate Limiting Bypass\",\n        \"Shadow Parameter Exploitation\",\n        \"Unknown\"\n      ]\n    },\n    \"severity\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Severity level of the attack\",\n      \"enum\": [\"critical\", \"high\", \"medium\", \"low\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the attack\",\n      \"enum\": [\"active\", \"blocked\", \"resolved\", \"investigating\"]\n    },\n    \"source_ip\": {\n      \"type\": \"string\",\n      \"description\": \"Source IP address of the attacker\"\n    },\n    \"target_endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"API endpoint being attacked\"\n    },\n    \"target_api_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the API being attacked\"\n    },\n    \"attack_signature\": {\n      \"type\": \"string\",\n      \"description\": \"Pattern or signature that identified this as an attack\"\n    },\n    \"request_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of malicious requests in this attack\"\n    },\n\
  \    \"affected_users\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"User IDs or identifiers affected by this attack\"\n    },\n    \"data_exposed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether sensitive data was potentially exposed\"\n    },\n    \"mitigation_actions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"action\": {\n            \"type\": \"string\",\n            \"description\": \"Mitigation action taken (e.g., block, alert, rate-limit)\"\n          },\n          \"timestamp\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    },\n    \"remediation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"recommendation\": {\n          \"type\": \"string\",\n          \"description\": \"Developer-friendly remediation recommendation\"\
  \n        },\n        \"cwe\": {\n          \"type\": \"string\",\n          \"description\": \"Related CWE identifier\"\n        },\n        \"owasp\": {\n          \"type\": \"string\",\n          \"description\": \"Related OWASP API Security Top 10 category\"\n        }\n      }\n    },\n    \"detected_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when attack was first detected\"\n    },\n    \"resolved_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when attack was resolved\"\n    }\n  },\n  \"required\": [\"id\", \"attack_type\", \"severity\", \"target_endpoint\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salt-security/refs/heads/main/json-schema/salt-security-attack-schema.json
tags:
- API Security
- AI
- API Discovery
- Posture Governance
- Threat Protection
- Security
title: Salt Security API Attack
---
