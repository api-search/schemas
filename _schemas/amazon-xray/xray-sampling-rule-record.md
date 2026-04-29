---
description: A <a href="https://docs.aws.amazon.com/xray/latest/api/API_SamplingRule.html">SamplingRule</a> and its metadata.
layout: schema
name: SamplingRuleRecord
properties_list:
- description: ''
  name: SamplingRule
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: ModifiedAt
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-sampling-rule-record-schema.json
slug: xray-sampling-rule-record
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SamplingRule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamplingRule\"\n        },\n        {\n          \"description\": \"The sampling rule.\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"When the rule was created.\"\n        }\n      ]\n    },\n    \"ModifiedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"When the rule was last modified.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A <a href=\\\"https://docs.aws.amazon.com/xray/latest/api/API_SamplingRule.html\\\">SamplingRule</a> and its metadata.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SamplingRuleRecord\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-sampling-rule-record-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-sampling-rule-record-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: SamplingRuleRecord
---
