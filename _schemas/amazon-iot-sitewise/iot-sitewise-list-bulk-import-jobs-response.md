---
description: ListBulkImportJobsResponse schema
layout: schema
name: ListBulkImportJobsResponse
properties_list:
- description: ''
  name: jobSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-list-bulk-import-jobs-response-schema.json
slug: iot-sitewise-list-bulk-import-jobs-response
source_filename: iot-sitewise-list-bulk-import-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-list-bulk-import-jobs-response-schema.json\",\n  \"title\": \"ListBulkImportJobsResponse\",\n  \"description\": \"ListBulkImportJobsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobSummaries\"\n        },\n        {\n          \"description\": \"One or more job summaries to list.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token for the next set of results, or null if there are no additional results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jobSummaries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-list-bulk-import-jobs-response-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: ListBulkImportJobsResponse
---
