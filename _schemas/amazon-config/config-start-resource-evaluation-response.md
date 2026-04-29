---
description: StartResourceEvaluationResponse schema
layout: schema
name: StartResourceEvaluationResponse
properties_list:
- description: ''
  name: ResourceEvaluationId
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-start-resource-evaluation-response-schema.json
slug: config-start-resource-evaluation-response
source_filename: config-start-resource-evaluation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-start-resource-evaluation-response-schema.json\",\n  \"title\": \"StartResourceEvaluationResponse\",\n  \"description\": \"StartResourceEvaluationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceEvaluationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceEvaluationId\"\n        },\n        {\n          \"description\": \"A unique ResourceEvaluationId that is associated with a single execution.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-start-resource-evaluation-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: StartResourceEvaluationResponse
---
