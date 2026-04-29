---
description: EvaluationRequest schema from Amplitude Experiment Evaluation API
layout: schema
name: EvaluationRequest
properties_list:
- description: The user ID to evaluate experiments and flags for.
  name: user_id
  type: string
- description: The device ID to evaluate experiments and flags for.
  name: device_id
  type: string
- description: User properties to use for targeting rule evaluation.
  name: user_properties
  type: object
- description: Group type to group name mappings for group-level targeting.
  name: groups
  type: object
- description: Group properties to use for targeting rule evaluation.
  name: group_properties
  type: object
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/experiment-evaluation-api-evaluation-request-schema.json
slug: experiment-evaluation-api-evaluation-request
source_filename: experiment-evaluation-api-evaluation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-evaluation-api-evaluation-request-schema.json\",\n  \"title\": \"EvaluationRequest\",\n  \"description\": \"EvaluationRequest schema from Amplitude Experiment Evaluation API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"The user ID to evaluate experiments and flags for.\"\n    },\n    \"device_id\": {\n      \"type\": \"string\",\n      \"description\": \"The device ID to evaluate experiments and flags for.\"\n    },\n    \"user_properties\": {\n      \"type\": \"object\",\n      \"description\": \"User properties to use for targeting rule evaluation.\",\n      \"additionalProperties\": true\n    },\n    \"groups\": {\n      \"type\": \"object\",\n      \"description\": \"Group type to group name mappings for group-level\
  \ targeting.\",\n      \"additionalProperties\": true\n    },\n    \"group_properties\": {\n      \"type\": \"object\",\n      \"description\": \"Group properties to use for targeting rule evaluation.\",\n      \"additionalProperties\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/experiment-evaluation-api-evaluation-request-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: EvaluationRequest
---
