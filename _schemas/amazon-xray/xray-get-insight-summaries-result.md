---
description: GetInsightSummariesResult schema from Amazon X-Ray API
layout: schema
name: GetInsightSummariesResult
properties_list:
- description: ''
  name: InsightSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-insight-summaries-result-schema.json
slug: xray-get-insight-summaries-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"InsightSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightSummaryList\"\n        },\n        {\n          \"description\": \"The summary of each insight within the group matching the provided filters. The summary contains the InsightID, start and end time, the root cause service, the root cause and client impact statistics, the top anomalous services, and the status of the insight.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"Pagination token.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetInsightSummariesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-insight-summaries-result-schema.json\"\
  ,\n  \"description\": \"GetInsightSummariesResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-insight-summaries-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetInsightSummariesResult
---
