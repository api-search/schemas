---
description: <p/>
layout: schema
name: DeleteEvaluationResultsRequest
properties_list:
- description: ''
  name: ConfigRuleName
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-delete-evaluation-results-request-schema.json
slug: config-delete-evaluation-results-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-evaluation-results-request-schema.json\",\n  \"title\": \"DeleteEvaluationResultsRequest\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigRuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit64\"\n        },\n        {\n          \"description\": \"The name of the Config rule for which you want to delete the evaluation results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigRuleName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-delete-evaluation-results-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: DeleteEvaluationResultsRequest
---
