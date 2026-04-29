---
description: Request to change multiple seat licenses
layout: schema
name: BulkSeatChangeRequest
properties_list:
- description: List of seat changes (max 100 per request)
  name: seats
  type: array
provider_name: Backupify
provider_slug: backupify
schema_file: json-schema/saas-protection-api-bulk-seat-change-request-schema.json
slug: saas-protection-api-bulk-seat-change-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-bulk-seat-change-request-schema.json\",\n  \"title\": \"BulkSeatChangeRequest\",\n  \"description\": \"Request to change multiple seat licenses\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"seats\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SeatChange\"\n      },\n      \"description\": \"List of seat changes (max 100 per request)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-bulk-seat-change-request-schema.json
tags:
- SaaS Backup
- Data Protection
- Cloud Backup
- Microsoft 365
- Google Workspace
title: BulkSeatChangeRequest
---
