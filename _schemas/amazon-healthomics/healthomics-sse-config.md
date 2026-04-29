---
description: Server-side encryption (SSE) settings for a store.
layout: schema
name: SseConfig
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: keyArn
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-sse-config-schema.json
slug: healthomics-sse-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-sse-config-schema.json\",\n  \"title\": \"SseConfig\",\n  \"type\": \"object\",\n  \"required\": [\n    \"type\"\n  ],\n  \"properties\": {\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionType\"\n        },\n        {\n          \"description\": \"The encryption type.\"\n        }\n      ]\n    },\n    \"keyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SseConfigKeyArnString\"\n        },\n        {\n          \"description\": \"An encryption key ARN.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Server-side encryption (SSE) settings for a store.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-sse-config-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: SseConfig
---
