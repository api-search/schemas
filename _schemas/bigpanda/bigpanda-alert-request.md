---
description: Payload for ingesting a monitoring alert.
layout: schema
name: AlertRequest
properties_list:
- description: BigPanda application key for routing.
  name: app_key
  type: string
- description: Alert status.
  name: status
  type: string
- description: Hostname associated with the alert.
  name: host
  type: string
- description: Check or metric name that triggered the alert.
  name: check
  type: string
- description: Human-readable alert description.
  name: description
  type: string
- description: Unix timestamp of the alert.
  name: timestamp
  type: integer
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-alert-request-schema.json
slug: bigpanda-alert-request
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AlertRequest\",\n  \"type\": \"object\",\n  \"description\": \"Payload for ingesting a monitoring alert.\",\n  \"properties\": {\n    \"app_key\": {\n      \"type\": \"string\",\n      \"description\": \"BigPanda application key for routing.\",\n      \"example\": \"abc123appkey\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Alert status.\",\n      \"enum\": [\n        \"critical\",\n        \"warning\",\n        \"ok\",\n        \"acknowledged\"\n      ],\n      \"example\": \"critical\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname associated with the alert.\",\n      \"example\": \"production-database-1\"\n    },\n    \"check\": {\n      \"type\": \"string\",\n      \"description\": \"Check or metric name that triggered the alert.\",\n      \"example\": \"CPU overloaded\"\n    },\n    \"description\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Human-readable alert description.\",\n      \"example\": \"CPU usage above 95% for 5 minutes\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of the alert.\",\n      \"example\": 1713000000\n    }\n  },\n  \"required\": [\n    \"app_key\",\n    \"status\",\n    \"host\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/json-schema/bigpanda-alert-request-schema.json
tags:
- Incidents
- Monitoring
- Platform
title: AlertRequest
---
