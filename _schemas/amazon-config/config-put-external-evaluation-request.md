---
description: PutExternalEvaluationRequest schema
layout: schema
name: PutExternalEvaluationRequest
properties_list:
- description: ''
  name: ConfigRuleName
  type: object
- description: ''
  name: ExternalEvaluation
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-external-evaluation-request-schema.json
slug: config-put-external-evaluation-request
source_filename: config-put-external-evaluation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-external-evaluation-request-schema.json\",\n  \"title\": \"PutExternalEvaluationRequest\",\n  \"description\": \"PutExternalEvaluationRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigRuleName\"\n        },\n        {\n          \"description\": \"The name of the Config rule.\"\n        }\n      ]\n    },\n    \"ExternalEvaluation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalEvaluation\"\n        },\n        {\n          \"description\": \"An <code>ExternalEvaluation</code> object that provides details about compliance.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigRuleName\",\n    \"ExternalEvaluation\"\n  ]\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-external-evaluation-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: PutExternalEvaluationRequest
---
