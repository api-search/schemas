---
description: CreatePackageImportJobResponse schema from Amazon Panorama
layout: schema
name: CreatePackageImportJobResponse
properties_list:
- description: ''
  name: JobId
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-create-package-import-job-response-schema.json
slug: openapi-create-package-import-job-response
source_filename: openapi-create-package-import-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-package-import-job-response-schema.json\",\n  \"title\": \"CreatePackageImportJobResponse\",\n  \"description\": \"CreatePackageImportJobResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The job's ID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-package-import-job-response-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: CreatePackageImportJobResponse
---
