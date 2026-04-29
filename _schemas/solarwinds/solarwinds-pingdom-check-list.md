---
description: ''
layout: schema
name: CheckList
properties_list:
- description: ''
  name: checks
  type: array
- description: ''
  name: counts
  type: object
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-pingdom-check-list-schema.json
slug: solarwinds-pingdom-check-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CheckList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checks\": {\n      \"type\": \"array\"\n    },\n    \"counts\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-pingdom-check-list-schema.json
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
title: CheckList
---
