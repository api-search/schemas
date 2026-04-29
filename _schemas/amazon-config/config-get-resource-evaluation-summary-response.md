---
description: GetResourceEvaluationSummaryResponse schema
layout: schema
name: GetResourceEvaluationSummaryResponse
properties_list:
- description: ''
  name: ResourceEvaluationId
  type: object
- description: ''
  name: EvaluationMode
  type: object
- description: ''
  name: EvaluationStatus
  type: object
- description: ''
  name: EvaluationStartTimestamp
  type: object
- description: ''
  name: Compliance
  type: object
- description: ''
  name: EvaluationContext
  type: object
- description: ''
  name: ResourceDetails
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-resource-evaluation-summary-response-schema.json
slug: config-get-resource-evaluation-summary-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-resource-evaluation-summary-response-schema.json\",\n  \"title\": \"GetResourceEvaluationSummaryResponse\",\n  \"description\": \"GetResourceEvaluationSummaryResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceEvaluationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceEvaluationId\"\n        },\n        {\n          \"description\": \"The unique <code>ResourceEvaluationId</code> of Amazon Web Services resource execution for which you want to retrieve the evaluation summary.\"\n        }\n      ]\n    },\n    \"EvaluationMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationMode\"\n        },\n        {\n          \"description\": \"Lists results of the mode that you requested to retrieve\
  \ the resource evaluation summary. The valid values are Detective or Proactive.\"\n        }\n      ]\n    },\n    \"EvaluationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationStatus\"\n        },\n        {\n          \"description\": \"Returns an <code>EvaluationStatus</code> object.\"\n        }\n      ]\n    },\n    \"EvaluationStartTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The start timestamp when Config rule starts evaluating compliance for the provided resource details.\"\n        }\n      ]\n    },\n    \"Compliance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComplianceType\"\n        },\n        {\n          \"description\": \"The compliance status of the resource evaluation summary.\"\n        }\n      ]\n    },\n    \"EvaluationContext\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/EvaluationContext\"\n        },\n        {\n          \"description\": \"Returns an <code>EvaluationContext</code> object.\"\n        }\n      ]\n    },\n    \"ResourceDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceDetails\"\n        },\n        {\n          \"description\": \"Returns a <code>ResourceDetails</code> object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-resource-evaluation-summary-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetResourceEvaluationSummaryResponse
---
