---
description: DescribeExportTasksResponse schema from Amazon Application Discovery Service API
layout: schema
name: DescribeExportTasksResponse
properties_list:
- description: Contains one or more sets of export request details.
  name: exportsInfo
  type: array
- description: The nextToken value to include in a future DescribeExportTasks request.
  name: nextToken
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-describe-export-tasks-response-schema.json
slug: application-discovery-service-describe-export-tasks-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-export-tasks-response-schema.json\",\n  \"title\": \"DescribeExportTasksResponse\",\n  \"description\": \"DescribeExportTasksResponse schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exportsInfo\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"exportId\": {\n            \"type\": \"string\",\n            \"example\": \"export-500123\",\n            \"description\": \"A unique identifier used to query the status of an export request.\"\n          },\n          \"exportStatus\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"FAILED\",\n              \"SUCCEEDED\",\n              \"\
  IN_PROGRESS\"\n            ],\n            \"example\": \"SUCCEEDED\",\n            \"description\": \"The status of the data export job.\"\n          },\n          \"statusMessage\": {\n            \"type\": \"string\",\n            \"example\": \"Export complete\",\n            \"description\": \"A status message provided for API callers.\"\n          },\n          \"configurationsDownloadUrl\": {\n            \"type\": \"string\",\n            \"example\": \"https://s3.amazonaws.com/aws-application-discovery-service-export/500123/export.zip\",\n            \"description\": \"A URL for an Amazon S3 bucket where you can review the exported data.\"\n          },\n          \"exportRequestTime\": {\n            \"type\": \"string\",\n            \"example\": \"2026-04-19T10:00:00Z\",\n            \"description\": \"The time that the data export was initiated.\"\n          },\n          \"isTruncated\": {\n            \"type\": \"boolean\",\n            \"example\": false,\n            \"\
  description\": \"If true, the export of agent information exceeded the size limit for a single export, and the exported data is incomplete.\"\n          },\n          \"requestedStartTime\": {\n            \"type\": \"string\",\n            \"example\": \"2026-04-01T00:00:00Z\",\n            \"description\": \"The value of startTime parameter in the StartExportTask request.\"\n          },\n          \"requestedEndTime\": {\n            \"type\": \"string\",\n            \"example\": \"2026-04-19T23:59:59Z\",\n            \"description\": \"The endTime used in the StartExportTask request. If no endTime was requested, this result does not appear in ExportInfo.\"\n          }\n        },\n        \"required\": [\n          \"exportId\",\n          \"exportStatus\",\n          \"statusMessage\",\n          \"exportRequestTime\"\n        ]\n      },\n      \"description\": \"Contains one or more sets of export request details.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n\
  \      \"example\": \"\",\n      \"description\": \"The nextToken value to include in a future DescribeExportTasks request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-describe-export-tasks-response-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: DescribeExportTasksResponse
---
