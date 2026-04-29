---
description: ''
layout: schema
name: AccountInfo
properties_list:
- description: Account ID
  name: id
  type: integer
- description: Account subdomain
  name: subdomain
  type: string
- description: Customer tokens
  name: tokens
  type: array
- description: ''
  name: subscription
  type: object
- description: ''
  name: users
  type: array
provider_name: SolarWinds
provider_slug: solarwinds
schema_file: json-schema/solarwinds-loggly-account-info-schema.json
slug: solarwinds-loggly-account-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Account ID\"\n    },\n    \"subdomain\": {\n      \"type\": \"string\",\n      \"description\": \"Account subdomain\"\n    },\n    \"tokens\": {\n      \"type\": \"array\",\n      \"description\": \"Customer tokens\"\n    },\n    \"subscription\": {\n      \"type\": \"object\"\n    },\n    \"users\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solarwinds/refs/heads/main/json-schema/solarwinds-loggly-account-info-schema.json
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
title: AccountInfo
---
