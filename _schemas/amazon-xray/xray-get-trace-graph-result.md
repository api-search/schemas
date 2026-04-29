---
description: GetTraceGraphResult schema from Amazon X-Ray API
layout: schema
name: GetTraceGraphResult
properties_list:
- description: ''
  name: Services
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-trace-graph-result-schema.json
slug: xray-get-trace-graph-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Services\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceList\"\n        },\n        {\n          \"description\": \"The services that have processed one of the specified requests.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Pagination token.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetTraceGraphResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-trace-graph-result-schema.json\",\n  \"description\": \"GetTraceGraphResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-trace-graph-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetTraceGraphResult
---
