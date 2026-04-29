---
description: ListSigningProfilesResponse schema from AWS Signer API
layout: schema
name: ListSigningProfilesResponse
properties_list:
- description: ''
  name: profiles
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-list-signing-profiles-response-schema.json
slug: amazon-signer-list-signing-profiles-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-list-signing-profiles-response-schema.json\",\n  \"title\": \"ListSigningProfilesResponse\",\n  \"description\": \"ListSigningProfilesResponse schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"profiles\": {\n      \"allOf\": [\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/SigningProfile\"\n          }\n        },\n        {\n          \"description\": \"A list of profiles that are available in the AWS account. This includes profiles with the status of <code>CANCELED</code> if the <code>includeCanceled</code> parameter is set to <code>true</code>.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n        \
  \  \"description\": \"Value for specifying the next set of paginated results to return.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-list-signing-profiles-response-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: ListSigningProfilesResponse
---
