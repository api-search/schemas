---
description: UserPoolClientListType schema from Amazon Cognito
layout: schema
name: UserPoolClientListType
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-user-pool-client-list-type-schema.json
slug: cognito-idp-user-pool-client-list-type
source_filename: cognito-idp-user-pool-client-list-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"ClientId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ClientIdType\"\n          },\n          {\n            \"description\": \"The ID of the client associated with the user pool.\"\n          }\n        ]\n      },\n      \"UserPoolId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/UserPoolIdType\"\n          },\n          {\n            \"description\": \"The user pool ID for the user pool where you want to describe the user pool client.\"\n          }\n        ]\n      },\n      \"ClientName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ClientNameType\"\n          },\n          {\n            \"description\": \"The client name from the user pool client description.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The description of the user\
  \ pool client.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-user-pool-client-list-type-schema.json\",\n  \"title\": \"UserPoolClientListType\",\n  \"description\": \"UserPoolClientListType schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-user-pool-client-list-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UserPoolClientListType
---
