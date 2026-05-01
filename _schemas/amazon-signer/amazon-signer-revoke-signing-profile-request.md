---
description: RevokeSigningProfileRequest schema from AWS Signer API
layout: schema
name: RevokeSigningProfileRequest
properties_list:
- description: ''
  name: profileVersion
  type: object
- description: ''
  name: reason
  type: object
- description: ''
  name: effectiveTime
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-revoke-signing-profile-request-schema.json
slug: amazon-signer-revoke-signing-profile-request
source_filename: amazon-signer-revoke-signing-profile-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-revoke-signing-profile-request-schema.json\",\n  \"title\": \"RevokeSigningProfileRequest\",\n  \"description\": \"RevokeSigningProfileRequest schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profileVersion\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-zA-Z0-9]{10}$\",\n          \"minLength\": 10,\n          \"maxLength\": 10\n        },\n        {\n          \"description\": \"The version of the signing profile to be revoked.\"\n        }\n      ]\n    },\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"minLength\": 1,\n          \"maxLength\": 500\n        },\n        {\n          \"description\": \"The reason for revoking a signing profile.\"\n        }\n\
  \      ]\n    },\n    \"effectiveTime\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"description\": \"A timestamp for when revocation of a Signing Profile should become effective. Signatures generated using the signing profile after this timestamp are not trusted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"profileVersion\",\n    \"reason\",\n    \"effectiveTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-revoke-signing-profile-request-schema.json
tags:
- Code Signing
- IoT
- Lambda
- Security
title: RevokeSigningProfileRequest
---
