---
description: PathRule schema from Palo Alto Networks Prisma SD-WAN API
layout: schema
name: PathRule
properties_list:
- description: Unique identifier for the path rule.
  name: id
  type: string
- description: Name of the path rule.
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Application identifiers this path rule applies to.
  name: app_filters
  type: array
- description: Ordered list of preferred WAN paths for traffic steering.
  name: preferred_paths
  type: array
- description: SLA thresholds that trigger path switching.
  name: sla_threshold
  type: object
- description: Whether the rule is active.
  name: enabled
  type: boolean
- description: Rule evaluation priority. Lower numbers are evaluated first.
  name: priority
  type: integer
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-sd-wan-api-path-rule-schema.json
slug: prisma-sd-wan-api-path-rule
source_filename: prisma-sd-wan-api-path-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PathRule\",\n  \"description\": \"PathRule schema from Palo Alto Networks Prisma SD-WAN API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-path-rule-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the path rule.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the path rule.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"app_filters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Application identifiers this path rule applies to.\"\n    },\n    \"preferred_paths\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\
  ,\n        \"properties\": {\n          \"label\": {\n            \"type\": \"string\",\n            \"description\": \"WAN interface label for the preferred path.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"active\",\n              \"backup\"\n            ],\n            \"description\": \"Whether this path is active or backup.\"\n          }\n        }\n      },\n      \"description\": \"Ordered list of preferred WAN paths for traffic steering.\"\n    },\n    \"sla_threshold\": {\n      \"type\": \"object\",\n      \"description\": \"SLA thresholds that trigger path switching.\",\n      \"properties\": {\n        \"latency_ms\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum acceptable latency in milliseconds.\"\n        },\n        \"packet_loss_pct\": {\n          \"type\": \"number\",\n          \"description\": \"Maximum acceptable packet loss percentage.\"\n        },\n        \"jitter_ms\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"Maximum acceptable jitter in milliseconds.\"\n        }\n      }\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Whether the rule is active.\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Rule evaluation priority. Lower numbers are evaluated first.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-sd-wan-api-path-rule-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: PathRule
---
