---
description: Request to list migration waves
layout: schema
name: ListWavesRequest
properties_list:
- description: filters
  name: filters
  type: string
- description: Maximum results to return
  name: maxResults
  type: integer
- description: Pagination token
  name: nextToken
  type: string
- description: Account ID for cross-account access
  name: accountID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-list-waves-request-schema.json
slug: application-migration-service-list-waves-request
source_filename: application-migration-service-list-waves-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-list-waves-request-schema.json\",\n  \"title\": \"ListWavesRequest\",\n  \"description\": \"Request to list migration waves\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"type\": \"string\",\n      \"description\": \"filters\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum results to return\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-list-waves-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: ListWavesRequest
---
