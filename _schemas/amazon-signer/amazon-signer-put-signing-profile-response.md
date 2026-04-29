---
description: PutSigningProfileResponse schema from AWS Signer API
layout: schema
name: PutSigningProfileResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: profileVersion
  type: object
- description: ''
  name: profileVersionArn
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-put-signing-profile-response-schema.json
slug: amazon-signer-put-signing-profile-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-put-signing-profile-response-schema.json\",\n  \"title\": \"PutSigningProfileResponse\",\n  \"description\": \"PutSigningProfileResponse schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the signing profile created.\"\n        }\n      ]\n    },\n    \"profileVersion\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-zA-Z0-9]{10}$\",\n          \"minLength\": 10,\n          \"maxLength\": 10\n        },\n        {\n          \"description\": \"The version of the signing profile being created.\"\n        }\n      ]\n    },\n    \"profileVersionArn\": {\n \
  \     \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"minLength\": 20,\n          \"maxLength\": 2048\n        },\n        {\n          \"description\": \"The signing profile ARN, including the profile version.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-put-signing-profile-response-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: PutSigningProfileResponse
---
