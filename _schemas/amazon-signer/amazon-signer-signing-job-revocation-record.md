---
description: Revocation information for a signing job.
layout: schema
name: SigningJobRevocationRecord
properties_list:
- description: ''
  name: reason
  type: object
- description: ''
  name: revokedAt
  type: object
- description: ''
  name: revokedBy
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-signing-job-revocation-record-schema.json
slug: amazon-signer-signing-job-revocation-record
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-job-revocation-record-schema.json\",\n  \"title\": \"SigningJobRevocationRecord\",\n  \"description\": \"Revocation information for a signing job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"A caller-supplied reason for revocation.\"\n        }\n      ]\n    },\n    \"revokedAt\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        {\n          \"description\": \"The time of revocation.\"\n        }\n      ]\n    },\n    \"revokedBy\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"The identity of the revoker.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-signing-job-revocation-record-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: SigningJobRevocationRecord
---
