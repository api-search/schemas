---
description: CreateUploadUrlResponse schema from Amazon CodeGuru Security
layout: schema
name: CreateUploadUrlResponse
properties_list:
- description: ''
  name: codeArtifactId
  type: object
- description: ''
  name: requestHeaders
  type: object
- description: ''
  name: s3Url
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-create-upload-url-response-schema.json
slug: amazon-codeguru-security-create-upload-url-response
source_filename: amazon-codeguru-security-create-upload-url-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-create-upload-url-response-schema.json\",\n  \"title\": \"CreateUploadUrlResponse\",\n  \"description\": \"CreateUploadUrlResponse schema from Amazon CodeGuru Security\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"codeArtifactId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"The identifier for the uploaded code resource. \"\n        }\n      ]\n    },\n    \"requestHeaders\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestHeaderMap\"\n        },\n        {\n          \"description\": \"A set of key-value pairs that contain the required headers when uploading your resource.\"\n        }\n      ]\n    },\n    \"s3Url\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/S3Url\"\n        },\n        {\n          \"description\": \"A pre-signed S3 URL. You can upload the code file you want to scan and add the required <code>requestHeaders</code> using any HTTP client.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"codeArtifactId\",\n    \"requestHeaders\",\n    \"s3Url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-create-upload-url-response-schema.json
tags:
- Amazon
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: CreateUploadUrlResponse
---
