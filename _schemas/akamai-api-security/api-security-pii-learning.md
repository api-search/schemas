---
description: Summarizes availability of PII learning.
layout: schema
name: pii-learning
properties_list:
- description: Enables PII learning.
  name: enablePiiLearning
  type: boolean
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-pii-learning-schema.json
slug: api-security-pii-learning
source_filename: api-security-pii-learning-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-pii-learning-schema.json\",\n  \"title\": \"pii-learning\",\n  \"description\": \"Summarizes availability of PII learning.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enablePiiLearning\": {\n      \"description\": \"Enables PII learning.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"enablePiiLearning\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-pii-learning-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: pii-learning
---
