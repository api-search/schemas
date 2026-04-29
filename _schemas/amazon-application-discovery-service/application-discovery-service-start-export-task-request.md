---
description: StartExportTaskRequest schema from Amazon Application Discovery Service API
layout: schema
name: StartExportTaskRequest
properties_list:
- description: 'The file format for the returned export data. Default(s) are CSV. Note: The GRAPHML option has been deprecated.'
  name: exportDataFormat
  type: array
- description: If a filter is present, it selects the single agentId of the Application Discovery Agent for which data is exported.
  name: filters
  type: array
- description: The start timestamp for exported data from the single Application Discovery Agent selected in the filters.
  name: startTime
  type: string
- description: The end timestamp for exported data from the single Application Discovery Agent selected in the filters.
  name: endTime
  type: string
- description: Indicates the type of agent export.
  name: preferences
  type: object
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-start-export-task-request-schema.json
slug: application-discovery-service-start-export-task-request
source_filename: application-discovery-service-start-export-task-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-start-export-task-request-schema.json\",\n  \"title\": \"StartExportTaskRequest\",\n  \"description\": \"StartExportTaskRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exportDataFormat\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"CSV\"\n        ]\n      },\n      \"example\": [\n        \"CSV\"\n      ],\n      \"description\": \"The file format for the returned export data. Default(s) are CSV. Note: The GRAPHML option has been deprecated.\"\n    },\n    \"filters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\"\
  : \"string\",\n            \"example\": \"agentIds\",\n            \"description\": \"A single ExportFilter name. Supported filters \\u2014 agentIds.\"\n          },\n          \"values\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"example\": [\n              \"d-agent-500123\"\n            ],\n            \"description\": \"A single agent ID for a Discovery Agent. An agent ID can be found using the DescribeAgents action.\"\n          },\n          \"condition\": {\n            \"type\": \"string\",\n            \"example\": \"EQUALS\",\n            \"description\": \"Supported condition \\u2014 EQUALS.\"\n          }\n        },\n        \"required\": [\n          \"name\",\n          \"values\",\n          \"condition\"\n        ]\n      },\n      \"description\": \"If a filter is present, it selects the single agentId of the Application Discovery Agent for which data is exported.\"\n    },\n    \"\
  startTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-01T00:00:00Z\",\n      \"description\": \"The start timestamp for exported data from the single Application Discovery Agent selected in the filters.\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-19T23:59:59Z\",\n      \"description\": \"The end timestamp for exported data from the single Application Discovery Agent selected in the filters.\"\n    },\n    \"preferences\": {\n      \"type\": \"object\",\n      \"description\": \"Indicates the type of agent export.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-start-export-task-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: StartExportTaskRequest
---
