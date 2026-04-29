---
description: BatchActivationRequest schema from AB Tasty Decision API
layout: schema
name: BatchActivationRequest
properties_list:
- description: Environment ID
  name: cid
  type: string
- description: ''
  name: batch
  type: array
provider_name: AB Tasty
provider_slug: ab-tasty
schema_file: json-schema/decision-api-batch-activation-request-schema.json
slug: decision-api-batch-activation-request
source_filename: decision-api-batch-activation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-batch-activation-request-schema.json\",\n  \"title\": \"BatchActivationRequest\",\n  \"description\": \"BatchActivationRequest schema from AB Tasty Decision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cid\": {\n      \"type\": \"string\",\n      \"description\": \"Environment ID\",\n      \"example\": \"env_abc\"\n    },\n    \"batch\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BatchActivationItem\"\n      },\n      \"minItems\": 1\n    }\n  },\n  \"required\": [\n    \"cid\",\n    \"batch\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-batch-activation-request-schema.json
tags:
- Aggregation
- Experimentation
- Feature Flags
- Personalization
- A/B Testing
title: BatchActivationRequest
---
