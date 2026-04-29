---
description: An asynchronous job tracking configuration push or commit operations.
layout: schema
name: Job
properties_list:
- description: Unique job identifier.
  name: id
  type: string
- description: Job type (e.g., push, commit).
  name: type
  type: string
- description: Current job status.
  name: status
  type: string
- description: ''
  name: result
  type: string
- description: Job start timestamp.
  name: start_ts
  type: string
- description: Job completion timestamp.
  name: end_ts
  type: string
- description: Job completion percentage (0-100).
  name: percent
  type: integer
- description: Additional job details and error messages.
  name: details
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/strata-cloud-manager-api-job-schema.json
slug: strata-cloud-manager-api-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Job\",\n  \"description\": \"An asynchronous job tracking configuration push or commit operations.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-job-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique job identifier.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Job type (e.g., push, commit).\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PEND\",\n        \"ACT\",\n        \"FIN\",\n        \"FAIL\"\n      ],\n      \"description\": \"Current job status.\"\n    },\n    \"result\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"OK\",\n        \"FAIL\",\n        \"WARN\"\n      ]\n    },\n    \"start_ts\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"Job start timestamp.\"\n    },\n    \"end_ts\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Job completion timestamp.\"\n    },\n    \"percent\": {\n      \"type\": \"integer\",\n      \"description\": \"Job completion percentage (0-100).\"\n    },\n    \"details\": {\n      \"type\": \"object\",\n      \"description\": \"Additional job details and error messages.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/strata-cloud-manager-api-job-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Job
---
