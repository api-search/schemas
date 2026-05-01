---
description: Revocation information for a signing profile.
layout: schema
name: SigningProfileRevocationRecord
properties_list:
- description: ''
  name: revocationEffectiveFrom
  type: object
- description: ''
  name: revokedAt
  type: object
- description: ''
  name: revokedBy
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-signing-profile-revocation-record-schema.json
slug: amazon-signer-signing-profile-revocation-record
source_filename: amazon-signer-signing-profile-revocation-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-profile-revocation-record-schema.json\",\n  \"title\": \"SigningProfileRevocationRecord\",\n  \"description\": \"Revocation information for a signing profile.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"revocationEffectiveFrom\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"description\": \"The time when revocation becomes effective.\"\n        }\n      ]\n    },\n    \"revokedAt\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"description\": \"The time when the signing profile was revoked.\"\n        }\n      ]\n    },\n    \"revokedBy\": {\n      \"allOf\": [\n        {\n          \"type\"\
  : \"string\"\n        },\n        {\n          \"description\": \"The identity of the revoker.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-profile-revocation-record-schema.json
tags:
- Code Signing
- IoT
- Lambda
- Security
title: SigningProfileRevocationRecord
---
