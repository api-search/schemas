---
description: ''
layout: schema
name: CreateVariantStoreResponse
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
  name: name
  type: object
- description: ''
  name: creationTime
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-create-variant-store-response-schema.json
slug: healthomics-create-variant-store-response
source_filename: healthomics-create-variant-store-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-variant-store-response-schema.json\",\n  \"title\": \"CreateVariantStoreResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"status\",\n    \"name\",\n    \"creationTime\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The store's ID.\"\n        }\n      ]\n    },\n    \"reference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceItem\"\n        },\n        {\n          \"description\": \"The store's genome reference.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StoreStatus\"\n        },\n        {\n        \
  \  \"description\": \"The store's status.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The store's name.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreationTime\"\n        },\n        {\n          \"description\": \"When the store was created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-variant-store-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: CreateVariantStoreResponse
---
