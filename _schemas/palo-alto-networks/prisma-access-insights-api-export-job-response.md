---
description: Response from a submitted export job
layout: schema
name: ExportJobResponse
properties_list:
- description: Unique identifier for the export job
  name: job_id
  type: string
- description: Current job status
  name: status
  type: string
- description: Job submission timestamp
  name: submitted_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-insights-api-export-job-response-schema.json
slug: prisma-access-insights-api-export-job-response
source_filename: prisma-access-insights-api-export-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExportJobResponse\",\n  \"description\": \"Response from a submitted export job\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-insights-api-export-job-response-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"job_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the export job\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING\",\n        \"RUNNING\",\n        \"COMPLETED\",\n        \"FAILED\"\n      ],\n      \"description\": \"Current job status\"\n    },\n    \"submitted_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Job submission timestamp\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-insights-api-export-job-response-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ExportJobResponse
---
