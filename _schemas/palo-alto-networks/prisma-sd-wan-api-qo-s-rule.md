---
description: QoSRule schema from Palo Alto Networks Prisma SD-WAN API
layout: schema
name: QoSRule
properties_list:
- description: Unique identifier for the QoS rule.
  name: id
  type: string
- description: Name of the QoS rule.
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Traffic priority for matching flows.
  name: priority
  type: string
- description: DSCP class to apply for marking traffic.
  name: dscp_class
  type: string
- description: Application names or identifiers this rule applies to.
  name: app_filters
  type: array
- description: Upstream bandwidth limit in Mbps for matched traffic.
  name: bandwidth_limit_up
  type: number
- description: Downstream bandwidth limit in Mbps for matched traffic.
  name: bandwidth_limit_down
  type: number
- description: Whether the rule is active.
  name: enabled
  type: boolean
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-sd-wan-api-qo-s-rule-schema.json
slug: prisma-sd-wan-api-qo-s-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"QoSRule\",\n  \"description\": \"QoSRule schema from Palo Alto Networks Prisma SD-WAN API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-qo-s-rule-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the QoS rule.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the QoS rule.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"high\",\n        \"medium\",\n        \"low\",\n        \"default\"\n      ],\n      \"description\": \"Traffic priority for matching flows.\"\n    },\n    \"dscp_class\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"DSCP class to apply for marking traffic.\"\n    },\n    \"app_filters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Application names or identifiers this rule applies to.\"\n    },\n    \"bandwidth_limit_up\": {\n      \"type\": \"number\",\n      \"description\": \"Upstream bandwidth limit in Mbps for matched traffic.\"\n    },\n    \"bandwidth_limit_down\": {\n      \"type\": \"number\",\n      \"description\": \"Downstream bandwidth limit in Mbps for matched traffic.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Whether the rule is active.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-qo-s-rule-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: QoSRule
---
