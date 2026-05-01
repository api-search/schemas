---
description: Use EvaluationContext to group independently initiated proactive resource evaluations. For example, CFN Stack. If you want to check just a resource definition, you do not need to provide evaluation context.
layout: schema
name: EvaluationContext
properties_list:
- description: ''
  name: EvaluationContextIdentifier
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-evaluation-context-schema.json
slug: config-evaluation-context
source_filename: config-evaluation-context-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-evaluation-context-schema.json\",\n  \"title\": \"EvaluationContext\",\n  \"description\": \"Use EvaluationContext to group independently initiated proactive resource evaluations. For example, CFN Stack. If you want to check just a resource definition, you do not need to provide evaluation context.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EvaluationContextIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationContextIdentifier\"\n        },\n        {\n          \"description\": \"A unique EvaluationContextIdentifier ID for an EvaluationContext.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-evaluation-context-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: EvaluationContext
---
