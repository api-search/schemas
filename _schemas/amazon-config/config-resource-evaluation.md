---
description: Returns details of a resource evaluation.
layout: schema
name: ResourceEvaluation
properties_list:
- description: ''
  name: ResourceEvaluationId
  type: object
- description: ''
  name: EvaluationMode
  type: object
- description: ''
  name: EvaluationStartTimestamp
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-resource-evaluation-schema.json
slug: config-resource-evaluation
source_filename: config-resource-evaluation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-evaluation-schema.json\",\n  \"title\": \"ResourceEvaluation\",\n  \"description\": \"Returns details of a resource evaluation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceEvaluationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceEvaluationId\"\n        },\n        {\n          \"description\": \"The ResourceEvaluationId of a evaluation.\"\n        }\n      ]\n    },\n    \"EvaluationMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationMode\"\n        },\n        {\n          \"description\": \"The mode of an evaluation. The valid values are Detective or Proactive.\"\n        }\n      ]\n    },\n    \"EvaluationStartTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The starting time of an execution.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-resource-evaluation-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: ResourceEvaluation
---
