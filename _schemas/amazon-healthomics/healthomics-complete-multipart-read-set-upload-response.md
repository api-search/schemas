---
description: ''
layout: schema
name: CompleteMultipartReadSetUploadResponse
properties_list:
- description: ''
  name: readSetId
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-complete-multipart-read-set-upload-response-schema.json
slug: healthomics-complete-multipart-read-set-upload-response
source_filename: healthomics-complete-multipart-read-set-upload-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-complete-multipart-read-set-upload-response-schema.json\",\n  \"title\": \"CompleteMultipartReadSetUploadResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"readSetId\"\n  ],\n  \"properties\": {\n    \"readSetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetId\"\n        },\n        {\n          \"description\": \" The read set ID created for an uploaded read set. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-complete-multipart-read-set-upload-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: CompleteMultipartReadSetUploadResponse
---
