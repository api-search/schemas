---
description: ''
layout: schema
name: CompleteMultipartReadSetUploadRequest
properties_list:
- description: ''
  name: parts
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-complete-multipart-read-set-upload-request-schema.json
slug: healthomics-complete-multipart-read-set-upload-request
source_filename: healthomics-complete-multipart-read-set-upload-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-complete-multipart-read-set-upload-request-schema.json\",\n  \"title\": \"CompleteMultipartReadSetUploadRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"parts\"\n  ],\n  \"properties\": {\n    \"parts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CompleteReadSetUploadPartList\"\n        },\n        {\n          \"description\": \" The individual uploads or parts of a multipart upload. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-complete-multipart-read-set-upload-request-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: CompleteMultipartReadSetUploadRequest
---
