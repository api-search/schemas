---
description: CreateUploadUrlRequest schema from Amazon CodeGuru Security
layout: schema
name: CreateUploadUrlRequest
properties_list:
- description: ''
  name: scanName
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-create-upload-url-request-schema.json
slug: amazon-codeguru-security-create-upload-url-request
source_filename: amazon-codeguru-security-create-upload-url-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-create-upload-url-request-schema.json\",\n  \"title\": \"CreateUploadUrlRequest\",\n  \"description\": \"CreateUploadUrlRequest schema from Amazon CodeGuru Security\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scanName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScanName\"\n        },\n        {\n          \"description\": \"The name of the scan that will use the uploaded resource. CodeGuru Security uses the unique scan name to track revisions across multiple scans of the same resource. Use this <code>scanName</code> when you call <code>CreateScan</code> on the code resource you upload to this URL.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"scanName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-create-upload-url-request-schema.json
tags:
- Amazon
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: CreateUploadUrlRequest
---
