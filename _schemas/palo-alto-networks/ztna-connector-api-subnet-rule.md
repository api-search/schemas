---
description: SubnetRule schema from Palo Alto Networks ZTNA Connector API
layout: schema
name: SubnetRule
properties_list:
- description: Unique identifier of the subnet rule.
  name: rule_id
  type: string
- description: Display name of the rule.
  name: name
  type: string
- description: CIDR notation subnet this rule covers (e.g., 10.0.0.0/8).
  name: subnet
  type: string
- description: Connector group used to route traffic to this subnet.
  name: group_id
  type: string
- description: Whether this rule is active.
  name: enabled
  type: boolean
- description: ''
  name: created_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/ztna-connector-api-subnet-rule-schema.json
slug: ztna-connector-api-subnet-rule
source_filename: ztna-connector-api-subnet-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubnetRule\",\n  \"description\": \"SubnetRule schema from Palo Alto Networks ZTNA Connector API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-subnet-rule-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rule_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the subnet rule.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the rule.\"\n    },\n    \"subnet\": {\n      \"type\": \"string\",\n      \"description\": \"CIDR notation subnet this rule covers (e.g., 10.0.0.0/8).\"\n    },\n    \"group_id\": {\n      \"type\": \"string\",\n      \"description\": \"Connector group used to route traffic to this subnet.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this\
  \ rule is active.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-subnet-rule-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: SubnetRule
---
