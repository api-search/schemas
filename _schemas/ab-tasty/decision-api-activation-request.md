---
description: ActivationRequest schema from AB Tasty Decision API
layout: schema
name: ActivationRequest
properties_list:
- description: Visitor ID
  name: vid
  type: string
- description: Anonymous ID (for experience continuity)
  name: aid
  type: string
- description: Environment ID
  name: cid
  type: string
- description: Variation group ID
  name: caid
  type: string
- description: Variation ID
  name: vaid
  type: string
provider_name: AB Tasty
provider_slug: ab-tasty
schema_file: json-schema/decision-api-activation-request-schema.json
slug: decision-api-activation-request
source_filename: decision-api-activation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-activation-request-schema.json\",\n  \"title\": \"ActivationRequest\",\n  \"description\": \"ActivationRequest schema from AB Tasty Decision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vid\": {\n      \"type\": \"string\",\n      \"description\": \"Visitor ID\",\n      \"example\": \"user123\"\n    },\n    \"aid\": {\n      \"type\": \"string\",\n      \"description\": \"Anonymous ID (for experience continuity)\",\n      \"example\": \"session_xyz\"\n    },\n    \"cid\": {\n      \"type\": \"string\",\n      \"description\": \"Environment ID\",\n      \"example\": \"env_abc\"\n    },\n    \"caid\": {\n      \"type\": \"string\",\n      \"description\": \"Variation group ID\",\n      \"example\": \"vg_123\"\n    },\n    \"vaid\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Variation ID\",\n      \"example\": \"var_456\"\n    }\n  },\n  \"required\": [\n    \"vid\",\n    \"cid\",\n    \"caid\",\n    \"vaid\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-activation-request-schema.json
tags:
- Aggregation
- Experimentation
- Feature Flags
- Personalization
- A/B Testing
title: ActivationRequest
---
