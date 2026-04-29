---
description: PostureCheck schema from Palo Alto Networks SaaS Security Posture Management API
layout: schema
name: PostureCheck
properties_list:
- description: Unique identifier of the posture check result.
  name: check_id
  type: string
- description: ID of the onboarded application this check applies to.
  name: app_id
  type: string
- description: Name of the security posture check.
  name: check_name
  type: string
- description: Category of the posture check.
  name: check_type
  type: string
- description: Severity level if the check fails.
  name: severity
  type: string
- description: Current result status of the check.
  name: status
  type: string
- description: Description of what the check evaluates.
  name: description
  type: string
- description: Step-by-step remediation guidance for failed checks.
  name: remediation
  type: string
- description: Compliance frameworks this check maps to (e.g., CIS, SOC2, ISO27001).
  name: compliance_frameworks
  type: array
- description: Timestamp when the check was last evaluated.
  name: last_evaluated_at
  type: string
- description: Justification text if the check is suppressed.
  name: suppression_justification
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sspm-api-posture-check-schema.json
slug: sspm-api-posture-check
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PostureCheck\",\n  \"description\": \"PostureCheck schema from Palo Alto Networks SaaS Security Posture Management API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sspm-api-posture-check-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"check_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the posture check result.\"\n    },\n    \"app_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the onboarded application this check applies to.\"\n    },\n    \"check_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the security posture check.\"\n    },\n    \"check_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"access_control\",\n        \"authentication\",\n        \"data_protection\",\n        \"logging\",\n        \"\
  network_security\",\n        \"configuration\"\n      ],\n      \"description\": \"Category of the posture check.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"informational\",\n        \"low\",\n        \"medium\",\n        \"high\",\n        \"critical\"\n      ],\n      \"description\": \"Severity level if the check fails.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pass\",\n        \"fail\",\n        \"error\",\n        \"suppressed\"\n      ],\n      \"description\": \"Current result status of the check.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what the check evaluates.\"\n    },\n    \"remediation\": {\n      \"type\": \"string\",\n      \"description\": \"Step-by-step remediation guidance for failed checks.\"\n    },\n    \"compliance_frameworks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n \
  \     },\n      \"description\": \"Compliance frameworks this check maps to (e.g., CIS, SOC2, ISO27001).\"\n    },\n    \"last_evaluated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the check was last evaluated.\"\n    },\n    \"suppression_justification\": {\n      \"type\": \"string\",\n      \"description\": \"Justification text if the check is suppressed.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sspm-api-posture-check-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: PostureCheck
---
