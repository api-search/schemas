---
description: Response with list of export errors
layout: schema
name: ListExportErrorsResponse
properties_list:
- description: List of export errors
  name: items
  type: array
- description: Pagination token
  name: nextToken
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-list-export-errors-response-schema.json
slug: application-migration-service-list-export-errors-response
source_filename: application-migration-service-list-export-errors-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-list-export-errors-response-schema.json\",\n  \"title\": \"ListExportErrorsResponse\",\n  \"description\": \"Response with list of export errors\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"List of export errors\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-list-export-errors-response-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: ListExportErrorsResponse
---
