---
description: ListSigningPlatformsResponse schema from AWS Signer API
layout: schema
name: ListSigningPlatformsResponse
properties_list:
- description: ''
  name: platforms
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-list-signing-platforms-response-schema.json
slug: amazon-signer-list-signing-platforms-response
source_filename: amazon-signer-list-signing-platforms-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-list-signing-platforms-response-schema.json\",\n  \"title\": \"ListSigningPlatformsResponse\",\n  \"description\": \"ListSigningPlatformsResponse schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"platforms\": {\n      \"allOf\": [\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/SigningPlatform\"\n          }\n        },\n        {\n          \"description\": \"A list of all platforms that match the request parameters.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"Value for specifying the next set of paginated results to return.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-list-signing-platforms-response-schema.json
tags:
- Code Signing
- IoT
- Lambda
- Security
title: ListSigningPlatformsResponse
---
