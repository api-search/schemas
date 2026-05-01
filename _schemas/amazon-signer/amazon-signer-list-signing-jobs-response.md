---
description: ListSigningJobsResponse schema from AWS Signer API
layout: schema
name: ListSigningJobsResponse
properties_list:
- description: ''
  name: jobs
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-list-signing-jobs-response-schema.json
slug: amazon-signer-list-signing-jobs-response
source_filename: amazon-signer-list-signing-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-list-signing-jobs-response-schema.json\",\n  \"title\": \"ListSigningJobsResponse\",\n  \"description\": \"ListSigningJobsResponse schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobs\": {\n      \"allOf\": [\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/SigningJob\"\n          }\n        },\n        {\n          \"description\": \"A list of your signing jobs.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"String for specifying the next set of paginated results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-list-signing-jobs-response-schema.json
tags:
- Code Signing
- IoT
- Lambda
- Security
title: ListSigningJobsResponse
---
