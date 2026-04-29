---
description: BatchGetTracesResult schema from Amazon X-Ray API
layout: schema
name: BatchGetTracesResult
properties_list:
- description: ''
  name: Traces
  type: object
- description: ''
  name: UnprocessedTraceIds
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-batch-get-traces-result-schema.json
slug: xray-batch-get-traces-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Traces\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TraceList\"\n        },\n        {\n          \"description\": \"Full traces for the specified requests.\"\n        }\n      ]\n    },\n    \"UnprocessedTraceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnprocessedTraceIdList\"\n        },\n        {\n          \"description\": \"Trace IDs of requests that haven't been processed.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Pagination token.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchGetTracesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-batch-get-traces-result-schema.json\"\
  ,\n  \"description\": \"BatchGetTracesResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-batch-get-traces-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: BatchGetTracesResult
---
