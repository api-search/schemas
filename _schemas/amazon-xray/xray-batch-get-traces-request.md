---
description: BatchGetTracesRequest schema from Amazon X-Ray API
layout: schema
name: BatchGetTracesRequest
properties_list:
- description: ''
  name: TraceIds
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-batch-get-traces-request-schema.json
slug: xray-batch-get-traces-request
source_filename: xray-batch-get-traces-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"TraceIds\"\n  ],\n  \"title\": \"BatchGetTracesRequest\",\n  \"properties\": {\n    \"TraceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TraceIdList\"\n        },\n        {\n          \"description\": \"Specify the trace IDs of requests for which to retrieve segments.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Pagination token.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-batch-get-traces-request-schema.json\",\n  \"description\": \"BatchGetTracesRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-batch-get-traces-request-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: BatchGetTracesRequest
---
