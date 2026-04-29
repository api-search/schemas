---
description: ''
layout: schema
name: UploadReadSetPartResponse
properties_list:
- description: ''
  name: checksum
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-upload-read-set-part-response-schema.json
slug: healthomics-upload-read-set-part-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-upload-read-set-part-response-schema.json\",\n  \"title\": \"UploadReadSetPartResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"checksum\"\n  ],\n  \"properties\": {\n    \"checksum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" An identifier used to confirm that parts are being added to the intended upload. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-upload-read-set-part-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: UploadReadSetPartResponse
---
