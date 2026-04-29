---
description: Details about a reference store.
layout: schema
name: ReferenceStoreDetail
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: id
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
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-reference-store-detail-schema.json
slug: healthomics-reference-store-detail
source_filename: healthomics-reference-store-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-reference-store-detail-schema.json\",\n  \"title\": \"ReferenceStoreDetail\",\n  \"type\": \"object\",\n  \"required\": [\n    \"arn\",\n    \"id\",\n    \"creationTime\"\n  ],\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceStoreArn\"\n        },\n        {\n          \"description\": \"The store's ARN.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceStoreId\"\n        },\n        {\n          \"description\": \"The store's ID.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceStoreName\"\n        },\n        {\n          \"description\": \"The store's name.\"\
  \n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceStoreDescription\"\n        },\n        {\n          \"description\": \"The store's description.\"\n        }\n      ]\n    },\n    \"sseConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SseConfig\"\n        },\n        {\n          \"description\": \"The store's server-side encryption (SSE) settings.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"When the store was created.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Details about a reference store.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-reference-store-detail-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ReferenceStoreDetail
---
