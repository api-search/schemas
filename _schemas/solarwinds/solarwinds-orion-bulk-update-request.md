---
description: ''
layout: schema
name: BulkUpdateRequest
properties_list:
- description: Array of SWIS URIs to update
  name: uris
  type: array
- description: Properties to set on all specified entities
  name: properties
  type: object
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-orion-bulk-update-request-schema.json
slug: solarwinds-orion-bulk-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BulkUpdateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uris\": {\n      \"type\": \"array\",\n      \"description\": \"Array of SWIS URIs to update\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Properties to set on all specified entities\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-orion-bulk-update-request-schema.json
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
title: BulkUpdateRequest
---
