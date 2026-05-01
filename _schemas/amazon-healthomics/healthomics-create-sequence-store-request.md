---
description: ''
layout: schema
name: CreateSequenceStoreRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: sseConfig
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: fallbackLocation
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-create-sequence-store-request-schema.json
slug: healthomics-create-sequence-store-request
source_filename: healthomics-create-sequence-store-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-sequence-store-request-schema.json\",\n  \"title\": \"CreateSequenceStoreRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SequenceStoreName\"\n        },\n        {\n          \"description\": \"A name for the store.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SequenceStoreDescription\"\n        },\n        {\n          \"description\": \"A description for the store.\"\n        }\n      ]\n    },\n    \"sseConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SseConfig\"\n        },\n        {\n          \"description\": \"Server-side\
  \ encryption (SSE) settings for the store.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Tags for the store.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"To ensure that requests don't run multiple times, specify a unique token for each request.\"\n        }\n      ]\n    },\n    \"fallbackLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Destination\"\n        },\n        {\n          \"description\": \" An S3 location that is used to store files that have failed a direct upload. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-sequence-store-request-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: CreateSequenceStoreRequest
---
