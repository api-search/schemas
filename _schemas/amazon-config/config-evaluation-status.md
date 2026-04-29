---
description: Returns status details of an evaluation.
layout: schema
name: EvaluationStatus
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: FailureReason
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-evaluation-status-schema.json
slug: config-evaluation-status
source_filename: config-evaluation-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-evaluation-status-schema.json\",\n  \"title\": \"EvaluationStatus\",\n  \"description\": \"Returns status details of an evaluation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceEvaluationStatus\"\n        },\n        {\n          \"description\": \"The status of an execution. The valid values are In_Progress, Succeeded or Failed. \"\n        }\n      ]\n    },\n    \"FailureReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit1024\"\n        },\n        {\n          \"description\": \"An explanation for failed execution status.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-evaluation-status-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: EvaluationStatus
---
