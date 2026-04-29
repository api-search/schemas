---
description: FQDNRule schema from Palo Alto Networks ZTNA Connector API
layout: schema
name: FQDNRule
properties_list:
- description: Unique identifier of the FQDN rule.
  name: rule_id
  type: string
- description: Display name of the rule.
  name: name
  type: string
- description: FQDN pattern or wildcard (e.g., *.internal.example.com) that this rule matches.
  name: fqdn_pattern
  type: string
- description: Connector group used to resolve and access matching FQDNs.
  name: group_id
  type: string
- description: Ports covered by this rule.
  name: ports
  type: array
- description: Whether this rule is active.
  name: enabled
  type: boolean
- description: ''
  name: created_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/ztna-connector-api-fqdn-rule-schema.json
slug: ztna-connector-api-fqdn-rule
source_filename: ztna-connector-api-fqdn-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FQDNRule\",\n  \"description\": \"FQDNRule schema from Palo Alto Networks ZTNA Connector API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-fqdn-rule-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rule_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the FQDN rule.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the rule.\"\n    },\n    \"fqdn_pattern\": {\n      \"type\": \"string\",\n      \"description\": \"FQDN pattern or wildcard (e.g., *.internal.example.com) that this rule matches.\"\n    },\n    \"group_id\": {\n      \"type\": \"string\",\n      \"description\": \"Connector group used to resolve and access matching FQDNs.\"\n    },\n    \"ports\": {\n      \"type\": \"array\",\n      \"items\":\
  \ {\n        \"type\": \"integer\"\n      },\n      \"description\": \"Ports covered by this rule.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this rule is active.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/ztna-connector-api-fqdn-rule-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: FQDNRule
---
