---
description: ''
layout: schema
name: ListReadSetUploadPartsRequest
properties_list:
- description: ''
  name: partSource
  type: object
- description: ''
  name: filter
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-list-read-set-upload-parts-request-schema.json
slug: healthomics-list-read-set-upload-parts-request
source_filename: healthomics-list-read-set-upload-parts-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-read-set-upload-parts-request-schema.json\",\n  \"title\": \"ListReadSetUploadPartsRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"partSource\"\n  ],\n  \"properties\": {\n    \"partSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetPartSource\"\n        },\n        {\n          \"description\": \" The source file for the upload part. \"\n        }\n      ]\n    },\n    \"filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetUploadPartListFilter\"\n        },\n        {\n          \"description\": \" Attributes used to filter for a specific subset of read set part uploads. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-list-read-set-upload-parts-request-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ListReadSetUploadPartsRequest
---
