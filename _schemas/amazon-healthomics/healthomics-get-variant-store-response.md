---
description: ''
layout: schema
name: GetVariantStoreResponse
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: reference
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: storeArn
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
  name: updateTime
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: statusMessage
  type: object
- description: ''
  name: storeSizeBytes
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-get-variant-store-response-schema.json
slug: healthomics-get-variant-store-response
source_filename: healthomics-get-variant-store-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-variant-store-response-schema.json\",\n  \"title\": \"GetVariantStoreResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"reference\",\n    \"status\",\n    \"storeArn\",\n    \"name\",\n    \"description\",\n    \"sseConfig\",\n    \"creationTime\",\n    \"updateTime\",\n    \"tags\",\n    \"statusMessage\",\n    \"storeSizeBytes\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The store's ID.\"\n        }\n      ]\n    },\n    \"reference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceItem\"\n        },\n        {\n          \"description\": \"The store's genome reference.\"\n       \
  \ }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StoreStatus\"\n        },\n        {\n          \"description\": \"The store's status.\"\n        }\n      ]\n    },\n    \"storeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The store's ARN.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The store's name.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StoreDescription\"\n        },\n        {\n          \"description\": \"The store's description.\"\n        }\n      ]\n    },\n    \"sseConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SseConfig\"\n        },\n        {\n    \
  \      \"description\": \"The store's server-side encryption (SSE) settings.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreationTime\"\n        },\n        {\n          \"description\": \"When the store was created.\"\n        }\n      ]\n    },\n    \"updateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateTime\"\n        },\n        {\n          \"description\": \"When the store was updated.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The store's tags.\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusMessage\"\n        },\n        {\n          \"description\": \"The store's status message.\"\n        }\n      ]\n    },\n    \"storeSizeBytes\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The store's size in bytes.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-variant-store-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: GetVariantStoreResponse
---
