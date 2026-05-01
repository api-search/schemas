---
description: UpdateSamplingRuleResult schema from Amazon X-Ray API
layout: schema
name: UpdateSamplingRuleResult
properties_list:
- description: ''
  name: SamplingRuleRecord
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-update-sampling-rule-result-schema.json
slug: xray-update-sampling-rule-result
source_filename: xray-update-sampling-rule-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SamplingRuleRecord\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamplingRuleRecord\"\n        },\n        {\n          \"description\": \"The updated rule definition and metadata.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateSamplingRuleResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-update-sampling-rule-result-schema.json\",\n  \"description\": \"UpdateSamplingRuleResult schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-update-sampling-rule-result-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: UpdateSamplingRuleResult
---
