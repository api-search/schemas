---
description: The structure representing the ListFindingsReportsResponse.
layout: schema
name: ListFindingsReportsResponse
properties_list:
- description: ''
  name: findingsReportSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-list-findings-reports-response-schema.json
slug: amazon-codeguru-profiler-list-findings-reports-response
source_filename: amazon-codeguru-profiler-list-findings-reports-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-list-findings-reports-response-schema.json\",\n  \"title\": \"ListFindingsReportsResponse\",\n  \"description\": \"The structure representing the ListFindingsReportsResponse.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findingsReportSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingsReportSummaries\"\n        },\n        {\n          \"description\": \"The list of analysis results summaries.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> value to include in a future <code>ListFindingsReports</code> request. When the results of a <code>ListFindingsReports</code>\
  \ request exceed <code>maxResults</code>, this value can be used to retrieve the next page of results. This value is <code>null</code> when there are no more results to return.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"findingsReportSummaries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-list-findings-reports-response-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: ListFindingsReportsResponse
---
