---
description: AddProfilePermissionResponse schema from AWS Signer API
layout: schema
name: AddProfilePermissionResponse
properties_list:
- description: ''
  name: revisionId
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-add-profile-permission-response-schema.json
slug: amazon-signer-add-profile-permission-response
source_filename: amazon-signer-add-profile-permission-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-add-profile-permission-response-schema.json\",\n  \"title\": \"AddProfilePermissionResponse\",\n  \"description\": \"AddProfilePermissionResponse schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"revisionId\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"A unique identifier for the current profile revision.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-add-profile-permission-response-schema.json
tags:
- Code Signing
- IoT
- Lambda
- Security
title: AddProfilePermissionResponse
---
