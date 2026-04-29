---
description: ''
layout: schema
name: BulkDeleteRequest
properties_list:
- description: Array of SWIS URIs to delete
  name: uris
  type: array
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-orion-bulk-delete-request-schema.json
slug: solarwinds-orion-bulk-delete-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BulkDeleteRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uris\": {\n      \"type\": \"array\",\n      \"description\": \"Array of SWIS URIs to delete\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-orion-bulk-delete-request-schema.json
tags:
- Application Monitoring
- Database Monitoring
- Infrastructure
- IP Address Management
- IT Management
- ITSM
- Log Management
- Network Monitoring
- Observability
title: BulkDeleteRequest
---
