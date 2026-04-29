---
description: GetEncryptionKeyResponse schema
layout: schema
name: GetEncryptionKeyResponse
properties_list:
- description: ''
  name: kmsKeyId
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-get-encryption-key-response-schema.json
slug: inspector-get-encryption-key-response
source_filename: inspector-get-encryption-key-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-get-encryption-key-response-schema.json\",\n  \"title\": \"GetEncryptionKeyResponse\",\n  \"description\": \"GetEncryptionKeyResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyArn\"\n        },\n        {\n          \"description\": \"A kms key ID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"kmsKeyId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-get-encryption-key-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: GetEncryptionKeyResponse
---
