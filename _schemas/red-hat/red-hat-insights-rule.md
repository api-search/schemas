---
description: An Advisor rule that defines detection logic for a specific system issue, along with resolution steps and remediation guidance.
layout: schema
name: Rule
properties_list:
- description: The unique identifier of the rule.
  name: rule_id
  type: string
- description: A description of what the rule detects.
  name: description
  type: string
- description: Whether the rule is currently active.
  name: active
  type: boolean
- description: The category the rule belongs to.
  name: category
  type: object
- description: The impact level of the rule.
  name: impact
  type: object
- description: The likelihood value (1-4).
  name: likelihood
  type: integer
- description: The calculated total risk score.
  name: total_risk
  type: integer
- description: The risk associated with applying the remediation.
  name: risk_of_change
  type: integer
- description: Whether an Ansible remediation playbook is available.
  name: has_playbook
  type: boolean
- description: When the rule was published.
  name: publish_date
  type: string
- description: The number of systems currently affected by this rule.
  name: systems_affected
  type: integer
- description: Available resolution options for the rule.
  name: resolution_set
  type: array
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-insights-rule-schema.json
slug: red-hat-insights-rule
source_filename: red-hat-insights-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Rule\",\n  \"type\": \"object\",\n  \"description\": \"An Advisor rule that defines detection logic for a specific system issue, along with resolution steps and remediation guidance.\",\n  \"properties\": {\n    \"rule_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the rule.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of what the rule detects.\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the rule is currently active.\"\n    },\n    \"category\": {\n      \"type\": \"object\",\n      \"description\": \"The category the rule belongs to.\"\n    },\n    \"impact\": {\n      \"type\": \"object\",\n      \"description\": \"The impact level of the rule.\"\n    },\n    \"likelihood\": {\n      \"type\": \"integer\",\n      \"description\": \"The likelihood\
  \ value (1-4).\"\n    },\n    \"total_risk\": {\n      \"type\": \"integer\",\n      \"description\": \"The calculated total risk score.\"\n    },\n    \"risk_of_change\": {\n      \"type\": \"integer\",\n      \"description\": \"The risk associated with applying the remediation.\"\n    },\n    \"has_playbook\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether an Ansible remediation playbook is available.\"\n    },\n    \"publish_date\": {\n      \"type\": \"string\",\n      \"description\": \"When the rule was published.\"\n    },\n    \"systems_affected\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of systems currently affected by this rule.\"\n    },\n    \"resolution_set\": {\n      \"type\": \"array\",\n      \"description\": \"Available resolution options for the rule.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-insights-rule-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Rule
---
