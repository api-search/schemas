---
description: The structure representing the GetFindingsReportAccountSummaryResponse.
layout: schema
name: GetFindingsReportAccountSummaryResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: reportSummaries
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-get-findings-report-account-summary-response-schema.json
slug: amazon-codeguru-profiler-get-findings-report-account-summary-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-get-findings-report-account-summary-response-schema.json\",\n  \"title\": \"GetFindingsReportAccountSummaryResponse\",\n  \"description\": \"The structure representing the GetFindingsReportAccountSummaryResponse.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> value to include in a future <code>GetFindingsReportAccountSummary</code> request. When the results of a <code>GetFindingsReportAccountSummary</code> request exceed <code>maxResults</code>, this value can be used to retrieve the next page of results. This value is <code>null</code> when there are no more results to return.\"\
  \n        }\n      ]\n    },\n    \"reportSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingsReportSummaries\"\n        },\n        {\n          \"description\": \"The return list of <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_FindingsReportSummary.html\\\"> <code>FindingsReportSummary</code> </a> objects taht contain summaries of analysis results for all profiling groups in your AWS account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"reportSummaries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-get-findings-report-account-summary-response-schema.json
tags:
- Amazon
- AWS
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: GetFindingsReportAccountSummaryResponse
---
