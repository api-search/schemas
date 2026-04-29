---
description: Request to describe job log items
layout: schema
name: DescribeJobLogItemsRequest
properties_list:
- description: Job ID to get log items for
  name: jobID
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
schema_file: json-schema/application-migration-service-describe-job-log-items-request-schema.json
slug: application-migration-service-describe-job-log-items-request
source_filename: application-migration-service-describe-job-log-items-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-describe-job-log-items-request-schema.json\",\n  \"title\": \"DescribeJobLogItemsRequest\",\n  \"description\": \"Request to describe job log items\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobID\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID to get log items for\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum results to return\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-describe-job-log-items-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: DescribeJobLogItemsRequest
---
