---
description: ''
layout: schema
name: CreateVariantStoreRequest
properties_list:
- description: ''
  name: reference
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: sseConfig
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-create-variant-store-request-schema.json
slug: healthomics-create-variant-store-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-variant-store-request-schema.json\",\n  \"title\": \"CreateVariantStoreRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"reference\"\n  ],\n  \"properties\": {\n    \"reference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceItem\"\n        },\n        {\n          \"description\": \"The genome reference for the store's variants.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateVariantStoreRequestNameString\"\n        },\n        {\n          \"description\": \"A name for the store.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StoreDescription\"\n        },\n        {\n\
  \          \"description\": \"A description for the store.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Tags for the store.\"\n        }\n      ]\n    },\n    \"sseConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SseConfig\"\n        },\n        {\n          \"description\": \"Server-side encryption (SSE) settings for the store.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-variant-store-request-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: CreateVariantStoreRequest
---
