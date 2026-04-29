---
description: Payload for ingesting a change event.
layout: schema
name: ChangeRequest
properties_list:
- description: Human-readable change summary.
  name: summary
  type: string
- description: Change status.
  name: status
  type: string
- description: Unique change identifier.
  name: identifier
  type: string
- description: Hosts affected by the change.
  name: hosts
  type: array
- description: Unix timestamp of the change.
  name: timestamp
  type: integer
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-change-request-schema.json
slug: bigpanda-change-request
source_filename: bigpanda-change-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ChangeRequest\",\n  \"type\": \"object\",\n  \"description\": \"Payload for ingesting a change event.\",\n  \"properties\": {\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable change summary.\",\n      \"example\": \"Deployed v2.1.0 to production-database-1\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Change status.\",\n      \"enum\": [\n        \"started\",\n        \"success\",\n        \"failure\"\n      ],\n      \"example\": \"started\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"Unique change identifier.\",\n      \"example\": \"deploy-20240413-001\"\n    },\n    \"hosts\": {\n      \"type\": \"array\",\n      \"description\": \"Hosts affected by the change.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"production-database-1\"\
  \n      ]\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of the change.\",\n      \"example\": 1713000000\n    }\n  },\n  \"required\": [\n    \"summary\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/json-schema/bigpanda-change-request-schema.json
tags:
- Incidents
- Monitoring
- Platform
title: ChangeRequest
---
