---
description: List of audit log entries.
layout: schema
name: AuditLogsResponse
properties_list:
- description: Array of log entries.
  name: logs
  type: array
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-audit-logs-response-schema.json
slug: bigpanda-audit-logs-response
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AuditLogsResponse\",\n  \"type\": \"object\",\n  \"description\": \"List of audit log entries.\",\n  \"properties\": {\n    \"logs\": {\n      \"type\": \"array\",\n      \"description\": \"Array of log entries.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AuditLogEntry\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/json-schema/bigpanda-audit-logs-response-schema.json
tags:
- Incidents
- Monitoring
- Platform
title: AuditLogsResponse
---
