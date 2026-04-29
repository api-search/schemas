---
description: Results of bulk seat change operations
layout: schema
name: BulkSeatChangeResponse
properties_list:
- description: ''
  name: results
  type: array
provider_name: Backupify
provider_slug: backupify
schema_file: json-schema/saas-protection-api-bulk-seat-change-response-schema.json
slug: saas-protection-api-bulk-seat-change-response
source_filename: saas-protection-api-bulk-seat-change-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-bulk-seat-change-response-schema.json\",\n  \"title\": \"BulkSeatChangeResponse\",\n  \"description\": \"Results of bulk seat change operations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SeatChangeResult\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-bulk-seat-change-response-schema.json
tags:
- SaaS Backup
- Data Protection
- Cloud Backup
- Microsoft 365
- Google Workspace
title: BulkSeatChangeResponse
---
