---
description: RevokeSignatureRequest schema from AWS Signer API
layout: schema
name: RevokeSignatureRequest
properties_list:
- description: ''
  name: jobOwner
  type: object
- description: ''
  name: reason
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-revoke-signature-request-schema.json
slug: amazon-signer-revoke-signature-request
source_filename: amazon-signer-revoke-signature-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-revoke-signature-request-schema.json\",\n  \"title\": \"RevokeSignatureRequest\",\n  \"description\": \"RevokeSignatureRequest schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobOwner\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9]{12}$\",\n          \"minLength\": 12,\n          \"maxLength\": 12\n        },\n        {\n          \"description\": \"AWS account ID of the job owner.\"\n        }\n      ]\n    },\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 500\n        },\n        {\n          \"description\": \"The reason for revoking the signing job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"\
  reason\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-revoke-signature-request-schema.json
tags:
- Code Signing
- IoT
- Lambda
- Security
title: RevokeSignatureRequest
---
