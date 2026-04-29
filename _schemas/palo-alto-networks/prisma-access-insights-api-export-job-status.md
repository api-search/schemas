---
description: Status and result of an export job
layout: schema
name: ExportJobStatus
properties_list:
- description: Export job identifier
  name: job_id
  type: string
- description: Current job status
  name: status
  type: string
- description: Signed URL to download the export file (available when COMPLETED)
  name: download_url
  type: string
- description: Expiration time of the download URL
  name: expires_at
  type: string
- description: Error description if the job failed
  name: error_message
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-access-insights-api-export-job-status-schema.json
slug: prisma-access-insights-api-export-job-status
source_filename: prisma-access-insights-api-export-job-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExportJobStatus\",\n  \"description\": \"Status and result of an export job\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-insights-api-export-job-status-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"job_id\": {\n      \"type\": \"string\",\n      \"description\": \"Export job identifier\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING\",\n        \"RUNNING\",\n        \"COMPLETED\",\n        \"FAILED\"\n      ],\n      \"description\": \"Current job status\"\n    },\n    \"download_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Signed URL to download the export file (available when COMPLETED)\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Expiration time of the download URL\"\n    },\n    \"error_message\": {\n      \"type\": \"string\",\n      \"description\": \"Error description if the job failed\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-access-insights-api-export-job-status-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: ExportJobStatus
---
