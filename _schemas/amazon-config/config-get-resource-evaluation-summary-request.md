---
description: GetResourceEvaluationSummaryRequest schema
layout: schema
name: GetResourceEvaluationSummaryRequest
properties_list:
- description: ''
  name: ResourceEvaluationId
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-resource-evaluation-summary-request-schema.json
slug: config-get-resource-evaluation-summary-request
source_filename: config-get-resource-evaluation-summary-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-resource-evaluation-summary-request-schema.json\",\n  \"title\": \"GetResourceEvaluationSummaryRequest\",\n  \"description\": \"GetResourceEvaluationSummaryRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceEvaluationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceEvaluationId\"\n        },\n        {\n          \"description\": \"The unique <code>ResourceEvaluationId</code> of Amazon Web Services resource execution for which you want to retrieve the evaluation summary.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceEvaluationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-resource-evaluation-summary-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: GetResourceEvaluationSummaryRequest
---
