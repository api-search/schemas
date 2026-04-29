---
description: DescribeExportTasksRequest schema from Amazon Application Discovery Service API
layout: schema
name: DescribeExportTasksRequest
properties_list:
- description: One or more unique identifiers used to query the status of an export request.
  name: exportIds
  type: array
- description: One or more filters.
  name: filters
  type: array
- description: The maximum number of volume results returned by DescribeExportTasks in paginated output.
  name: maxResults
  type: integer
- description: The nextToken value returned from a previous paginated DescribeExportTasks request.
  name: nextToken
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-describe-export-tasks-request-schema.json
slug: application-discovery-service-describe-export-tasks-request
source_filename: application-discovery-service-describe-export-tasks-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-export-tasks-request-schema.json\",\n  \"title\": \"DescribeExportTasksRequest\",\n  \"description\": \"DescribeExportTasksRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exportIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"export-500123\"\n      ],\n      \"description\": \"One or more unique identifiers used to query the status of an export request.\"\n    },\n    \"filters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"agentIds\",\n           \
  \ \"description\": \"A single ExportFilter name. Supported filters \\u2014 agentIds.\"\n          },\n          \"values\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"example\": [\n              \"d-agent-500123\"\n            ],\n            \"description\": \"A single agent ID for a Discovery Agent. An agent ID can be found using the DescribeAgents action.\"\n          },\n          \"condition\": {\n            \"type\": \"string\",\n            \"example\": \"EQUALS\",\n            \"description\": \"Supported condition \\u2014 EQUALS.\"\n          }\n        },\n        \"required\": [\n          \"name\",\n          \"values\",\n          \"condition\"\n        ]\n      },\n      \"description\": \"One or more filters.\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"example\": 10,\n      \"description\": \"The maximum number of volume results returned by DescribeExportTasks\
  \ in paginated output.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"The nextToken value returned from a previous paginated DescribeExportTasks request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-export-tasks-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: DescribeExportTasksRequest
---
