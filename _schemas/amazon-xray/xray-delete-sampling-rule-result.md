---
description: DeleteSamplingRuleResult schema from Amazon X-Ray API
layout: schema
name: DeleteSamplingRuleResult
properties_list:
- description: ''
  name: SamplingRuleRecord
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-delete-sampling-rule-result-schema.json
slug: xray-delete-sampling-rule-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SamplingRuleRecord\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamplingRuleRecord\"\n        },\n        {\n          \"description\": \"The deleted rule definition and metadata.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteSamplingRuleResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-delete-sampling-rule-result-schema.json\",\n  \"description\": \"DeleteSamplingRuleResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-delete-sampling-rule-result-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: DeleteSamplingRuleResult
---
