---
description: UpdateSamplingRuleRequest schema from Amazon X-Ray API
layout: schema
name: UpdateSamplingRuleRequest
properties_list:
- description: ''
  name: SamplingRuleUpdate
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-update-sampling-rule-request-schema.json
slug: xray-update-sampling-rule-request
source_filename: xray-update-sampling-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"SamplingRuleUpdate\"\n  ],\n  \"title\": \"UpdateSamplingRuleRequest\",\n  \"properties\": {\n    \"SamplingRuleUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamplingRuleUpdate\"\n        },\n        {\n          \"description\": \"The rule and fields to change.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-update-sampling-rule-request-schema.json\",\n  \"description\": \"UpdateSamplingRuleRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-update-sampling-rule-request-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: UpdateSamplingRuleRequest
---
