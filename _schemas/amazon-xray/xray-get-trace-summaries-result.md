---
description: GetTraceSummariesResult schema from Amazon X-Ray API
layout: schema
name: GetTraceSummariesResult
properties_list:
- description: ''
  name: TraceSummaries
  type: object
- description: ''
  name: ApproximateTime
  type: object
- description: ''
  name: TracesProcessedCount
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-trace-summaries-result-schema.json
slug: xray-get-trace-summaries-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"TraceSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TraceSummaryList\"\n        },\n        {\n          \"description\": \"Trace IDs and annotations for traces that were found in the specified time frame.\"\n        }\n      ]\n    },\n    \"ApproximateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The start time of this page of results.\"\n        }\n      ]\n    },\n    \"TracesProcessedCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableLong\"\n        },\n        {\n          \"description\": \"The total number of traces processed, including traces that did not match the specified filter expression.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"If the requested time frame contained more than one page of results, you can use this token to retrieve the next page. The first page contains the most recent results, closest to the end of the time frame.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetTraceSummariesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-trace-summaries-result-schema.json\",\n  \"description\": \"GetTraceSummariesResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-trace-summaries-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetTraceSummariesResult
---
