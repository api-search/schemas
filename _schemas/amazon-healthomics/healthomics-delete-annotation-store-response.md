---
description: ''
layout: schema
name: DeleteAnnotationStoreResponse
properties_list:
- description: ''
  name: status
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-delete-annotation-store-response-schema.json
slug: healthomics-delete-annotation-store-response
source_filename: healthomics-delete-annotation-store-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-delete-annotation-store-response-schema.json\",\n  \"title\": \"DeleteAnnotationStoreResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"status\"\n  ],\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StoreStatus\"\n        },\n        {\n          \"description\": \"The store's status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-delete-annotation-store-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: DeleteAnnotationStoreResponse
---
