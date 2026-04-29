---
description: Request to get export errors
layout: schema
name: ExportErrorsRequest
properties_list:
- description: Export ID to get errors for
  name: exportID
  type: string
- description: Maximum results to return
  name: maxResults
  type: integer
- description: Pagination token
  name: nextToken
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-export-errors-request-schema.json
slug: application-migration-service-export-errors-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-export-errors-request-schema.json\",\n  \"title\": \"ExportErrorsRequest\",\n  \"description\": \"Request to get export errors\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exportID\": {\n      \"type\": \"string\",\n      \"description\": \"Export ID to get errors for\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum results to return\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-export-errors-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: ExportErrorsRequest
---
