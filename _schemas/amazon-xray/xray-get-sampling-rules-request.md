---
description: GetSamplingRulesRequest schema from Amazon X-Ray API
layout: schema
name: GetSamplingRulesRequest
properties_list:
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-sampling-rules-request-schema.json
slug: xray-get-sampling-rules-request
source_filename: xray-get-sampling-rules-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"GetSamplingRulesRequest\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Pagination token.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-sampling-rules-request-schema.json\",\n  \"description\": \"GetSamplingRulesRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-sampling-rules-request-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetSamplingRulesRequest
---
