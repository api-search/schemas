---
description: <p/>
layout: schema
name: StartConfigRulesEvaluationRequest
properties_list:
- description: ''
  name: ConfigRuleNames
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-start-config-rules-evaluation-request-schema.json
slug: config-start-config-rules-evaluation-request
source_filename: config-start-config-rules-evaluation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-start-config-rules-evaluation-request-schema.json\",\n  \"title\": \"StartConfigRulesEvaluationRequest\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReevaluateConfigRuleNames\"\n        },\n        {\n          \"description\": \"The list of names of Config rules that you want to run evaluations for.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-start-config-rules-evaluation-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: StartConfigRulesEvaluationRequest
---
