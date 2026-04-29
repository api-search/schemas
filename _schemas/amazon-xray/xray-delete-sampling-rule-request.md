---
description: DeleteSamplingRuleRequest schema from Amazon X-Ray API
layout: schema
name: DeleteSamplingRuleRequest
properties_list:
- description: ''
  name: RuleName
  type: object
- description: ''
  name: RuleARN
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-delete-sampling-rule-request-schema.json
slug: xray-delete-sampling-rule-request
source_filename: xray-delete-sampling-rule-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"title\": \"DeleteSamplingRuleRequest\",\n  \"properties\": {\n    \"RuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the sampling rule. Specify a rule by either name or ARN, but not both.\"\n        }\n      ]\n    },\n    \"RuleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ARN of the sampling rule. Specify a rule by either name or ARN, but not both.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-delete-sampling-rule-request-schema.json\",\n  \"description\": \"DeleteSamplingRuleRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-delete-sampling-rule-request-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: DeleteSamplingRuleRequest
---
