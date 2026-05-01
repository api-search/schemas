---
description: UnprocessedIdentityIdList schema from Amazon Cognito
layout: schema
name: UnprocessedIdentityIdList
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-unprocessed-identity-id-list-schema.json
slug: cognito-identity-unprocessed-identity-id-list
source_filename: cognito-identity-unprocessed-identity-id-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"IdentityId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IdentityId\"\n          },\n          {\n            \"description\": \"A unique identifier in the format REGION:GUID.\"\n          }\n        ]\n      },\n      \"ErrorCode\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ErrorCode\"\n          },\n          {\n            \"description\": \"The error code indicating the type of error that occurred.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An array of UnprocessedIdentityId objects, each of which contains an ErrorCode and IdentityId.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-unprocessed-identity-id-list-schema.json\",\n\
  \  \"title\": \"UnprocessedIdentityIdList\",\n  \"description\": \"UnprocessedIdentityIdList schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-unprocessed-identity-id-list-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UnprocessedIdentityIdList
---
