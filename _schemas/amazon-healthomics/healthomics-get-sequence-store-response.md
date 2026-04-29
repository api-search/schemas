---
description: ''
layout: schema
name: GetSequenceStoreResponse
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: arn
  type: object
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
  name: creationTime
  type: object
- description: ''
  name: fallbackLocation
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-get-sequence-store-response-schema.json
slug: healthomics-get-sequence-store-response
source_filename: healthomics-get-sequence-store-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-sequence-store-response-schema.json\",\n  \"title\": \"GetSequenceStoreResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"arn\",\n    \"creationTime\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SequenceStoreId\"\n        },\n        {\n          \"description\": \"The store's ID.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SequenceStoreArn\"\n        },\n        {\n          \"description\": \"The store's ARN.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SequenceStoreName\"\n        },\n        {\n          \"description\": \"The store's\
  \ name.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SequenceStoreDescription\"\n        },\n        {\n          \"description\": \"The store's description.\"\n        }\n      ]\n    },\n    \"sseConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SseConfig\"\n        },\n        {\n          \"description\": \"The store's server-side encryption (SSE) settings.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"When the store was created.\"\n        }\n      ]\n    },\n    \"fallbackLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Destination\"\n        },\n        {\n          \"description\": \" An S3 location that is used to store files that have failed a direct\
  \ upload. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-sequence-store-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: GetSequenceStoreResponse
---
