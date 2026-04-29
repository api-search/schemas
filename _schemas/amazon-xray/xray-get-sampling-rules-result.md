---
description: GetSamplingRulesResult schema from Amazon X-Ray API
layout: schema
name: GetSamplingRulesResult
properties_list:
- description: ''
  name: SamplingRuleRecords
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-get-sampling-rules-result-schema.json
slug: xray-get-sampling-rules-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SamplingRuleRecords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamplingRuleRecordList\"\n        },\n        {\n          \"description\": \"Rule definitions and metadata.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Pagination token.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetSamplingRulesResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-sampling-rules-result-schema.json\",\n  \"description\": \"GetSamplingRulesResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-get-sampling-rules-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: GetSamplingRulesResult
---
