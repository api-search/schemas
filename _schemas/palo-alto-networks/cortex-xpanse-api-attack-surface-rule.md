---
description: An attack surface rule defining criteria for classifying internet exposures as incidents.
layout: schema
name: AttackSurfaceRule
properties_list:
- description: ''
  name: attack_surface_rule_id
  type: string
- description: ''
  name: attack_surface_rule_name
  type: string
- description: Rule category (e.g., Unencrypted, Misconfigured, Unauthorized).
  name: category
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: remediation_guidance
  type: string
- description: ''
  name: enabled_status
  type: string
- description: ''
  name: severity
  type: string
- description: ''
  name: created
  type: integer
- description: ''
  name: modified
  type: integer
- description: ''
  name: release_status
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xpanse-api-attack-surface-rule-schema.json
slug: cortex-xpanse-api-attack-surface-rule
source_filename: cortex-xpanse-api-attack-surface-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AttackSurfaceRule\",\n  \"description\": \"An attack surface rule defining criteria for classifying internet exposures as incidents.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xpanse-api-attack-surface-rule-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attack_surface_rule_id\": {\n      \"type\": \"string\"\n    },\n    \"attack_surface_rule_name\": {\n      \"type\": \"string\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Rule category (e.g., Unencrypted, Misconfigured, Unauthorized).\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"remediation_guidance\": {\n      \"type\": \"string\"\n    },\n    \"enabled_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        true,\n        false\n      ]\n    },\n    \"severity\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\n        \"critical\",\n        \"high\",\n        \"medium\",\n        \"low\",\n        \"informational\"\n      ]\n    },\n    \"created\": {\n      \"type\": \"integer\"\n    },\n    \"modified\": {\n      \"type\": \"integer\"\n    },\n    \"release_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"GA\",\n        \"BETA\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xpanse-api-attack-surface-rule-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AttackSurfaceRule
---
