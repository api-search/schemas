---
description: Request to list source server lifecycle actions
layout: schema
name: ListSourceServerActionsRequest
properties_list:
- description: Source server ID
  name: sourceServerID
  type: string
- description: Action filters
  name: filters
  type: object
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
schema_file: json-schema/application-migration-service-list-source-server-actions-request-schema.json
slug: application-migration-service-list-source-server-actions-request
source_filename: application-migration-service-list-source-server-actions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-list-source-server-actions-request-schema.json\",\n  \"title\": \"ListSourceServerActionsRequest\",\n  \"description\": \"Request to list source server lifecycle actions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceServerID\": {\n      \"type\": \"string\",\n      \"description\": \"Source server ID\"\n    },\n    \"filters\": {\n      \"type\": \"object\",\n      \"description\": \"Action filters\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum results to return\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-list-source-server-actions-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: ListSourceServerActionsRequest
---
