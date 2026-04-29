---
description: An array of UnprocessedIdentityId objects, each of which contains an ErrorCode and IdentityId.
layout: schema
name: UnprocessedIdentityId
properties_list:
- description: ''
  name: IdentityId
  type: object
- description: ''
  name: ErrorCode
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-unprocessed-identity-id-schema.json
slug: identity-pools-unprocessed-identity-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-unprocessed-identity-id-schema.json\",\n  \"title\": \"UnprocessedIdentityId\",\n  \"description\": \"An array of UnprocessedIdentityId objects, each of which contains an ErrorCode and IdentityId.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityId\"\n        },\n        {\n          \"description\": \"A unique identifier in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorCode\"\n        },\n        {\n          \"description\": \"The error code indicating the type of error that occurred.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-unprocessed-identity-id-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: UnprocessedIdentityId
---
