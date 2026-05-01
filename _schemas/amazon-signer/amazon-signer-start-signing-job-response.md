---
description: StartSigningJobResponse schema from AWS Signer API
layout: schema
name: StartSigningJobResponse
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: jobOwner
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-start-signing-job-response-schema.json
slug: amazon-signer-start-signing-job-response
source_filename: amazon-signer-start-signing-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-start-signing-job-response-schema.json\",\n  \"title\": \"StartSigningJobResponse\",\n  \"description\": \"StartSigningJobResponse schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The ID of your signing job.\"\n        }\n      ]\n    },\n    \"jobOwner\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9]{12}$\",\n          \"minLength\": 12,\n          \"maxLength\": 12\n        },\n        {\n          \"description\": \"The AWS account ID of the signing job owner.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-start-signing-job-response-schema.json
tags:
- Code Signing
- IoT
- Lambda
- Security
title: StartSigningJobResponse
---
