---
description: ''
layout: schema
name: UpdateAnnotationStoreRequest
properties_list:
- description: ''
  name: description
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-update-annotation-store-request-schema.json
slug: healthomics-update-annotation-store-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-update-annotation-store-request-schema.json\",\n  \"title\": \"UpdateAnnotationStoreRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StoreDescription\"\n        },\n        {\n          \"description\": \"A description for the store.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-update-annotation-store-request-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: UpdateAnnotationStoreRequest
---
