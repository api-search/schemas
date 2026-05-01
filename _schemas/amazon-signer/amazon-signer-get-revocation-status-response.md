---
description: GetRevocationStatusResponse schema from AWS Signer API
layout: schema
name: GetRevocationStatusResponse
properties_list:
- description: ''
  name: revokedEntities
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-get-revocation-status-response-schema.json
slug: amazon-signer-get-revocation-status-response
source_filename: amazon-signer-get-revocation-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-get-revocation-status-response-schema.json\",\n  \"title\": \"GetRevocationStatusResponse\",\n  \"description\": \"GetRevocationStatusResponse schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"revokedEntities\": {\n      \"allOf\": [\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/String\"\n          }\n        },\n        {\n          \"description\": \"A list of revoked entities (including one or more of the signing profile ARN, signing job ID, and certificate hash) supplied as input to the API.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-get-revocation-status-response-schema.json
tags:
- Code Signing
- IoT
- Lambda
- Security
title: GetRevocationStatusResponse
---
