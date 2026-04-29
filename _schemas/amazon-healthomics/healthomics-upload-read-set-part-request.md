---
description: ''
layout: schema
name: UploadReadSetPartRequest
properties_list:
- description: ''
  name: payload
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-upload-read-set-part-request-schema.json
slug: healthomics-upload-read-set-part-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-upload-read-set-part-request-schema.json\",\n  \"title\": \"UploadReadSetPartRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"payload\"\n  ],\n  \"properties\": {\n    \"payload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetPartStreamingBlob\"\n        },\n        {\n          \"description\": \" The read set data to upload for a part. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-upload-read-set-part-request-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: UploadReadSetPartRequest
---
