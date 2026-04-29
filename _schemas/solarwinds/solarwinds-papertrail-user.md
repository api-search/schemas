---
description: ''
layout: schema
name: User
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: email
  type: string
- description: ''
  name: is_admin
  type: boolean
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-papertrail-user-schema.json
slug: solarwinds-papertrail-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"email\": {\n      \"type\": \"string\"\n    },\n    \"is_admin\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-papertrail-user-schema.json
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
title: User
---
