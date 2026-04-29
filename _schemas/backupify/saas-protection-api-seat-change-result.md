---
description: Result of a single seat change operation
layout: schema
name: SeatChangeResult
properties_list:
- description: Remote identifier for the seat
  name: remoteId
  type: string
- description: Whether the operation succeeded
  name: success
  type: boolean
- description: Description of the result
  name: message
  type: string
provider_name: Backupify
provider_slug: backupify
schema_file: json-schema/saas-protection-api-seat-change-result-schema.json
slug: saas-protection-api-seat-change-result
source_filename: saas-protection-api-seat-change-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-seat-change-result-schema.json\",\n  \"title\": \"SeatChangeResult\",\n  \"description\": \"Result of a single seat change operation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"remoteId\": {\n      \"type\": \"string\",\n      \"description\": \"Remote identifier for the seat\",\n      \"example\": \"user-abc123\"\n    },\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the operation succeeded\",\n      \"example\": true\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the result\",\n      \"example\": \"Seat licensed successfully\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/json-schema/saas-protection-api-seat-change-result-schema.json
tags:
- SaaS Backup
- Data Protection
- Cloud Backup
- Microsoft 365
- Google Workspace
title: SeatChangeResult
---
