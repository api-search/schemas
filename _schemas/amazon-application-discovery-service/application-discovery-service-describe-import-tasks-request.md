---
description: DescribeImportTasksRequest schema from Amazon Application Discovery Service API
layout: schema
name: DescribeImportTasksRequest
properties_list:
- description: An array of name-value pairs that you provide to filter the results for the DescribeImportTask request to a specific subset of results.
  name: filters
  type: array
- description: The maximum number of results that you want this request to return.
  name: maxResults
  type: integer
- description: The token to request a specific page of results.
  name: nextToken
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-describe-import-tasks-request-schema.json
slug: application-discovery-service-describe-import-tasks-request
source_filename: application-discovery-service-describe-import-tasks-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-import-tasks-request-schema.json\",\n  \"title\": \"DescribeImportTasksRequest\",\n  \"description\": \"DescribeImportTasksRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"IMPORT_TASK_ID\",\n              \"STATUS\",\n              \"NAME\"\n            ],\n            \"example\": \"STATUS\",\n            \"description\": \"The name, status, or import task ID for a specific import task.\"\n          },\n          \"values\": {\n            \"type\": \"array\",\n\
  \            \"items\": {\n              \"type\": \"string\"\n            },\n            \"example\": [\n              \"IMPORT_COMPLETE\"\n            ],\n            \"description\": \"An array of strings that you can provide to match against a specific name, status, or import task ID to filter your import task.\"\n          }\n        }\n      },\n      \"description\": \"An array of name-value pairs that you provide to filter the results for the DescribeImportTask request to a specific subset of results.\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 100,\n      \"example\": 10,\n      \"description\": \"The maximum number of results that you want this request to return.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"The token to request a specific page of results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-import-tasks-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
title: DescribeImportTasksRequest
---
