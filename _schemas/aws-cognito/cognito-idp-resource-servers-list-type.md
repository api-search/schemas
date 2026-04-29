---
description: ResourceServersListType schema from Amazon Cognito
layout: schema
name: ResourceServersListType
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-resource-servers-list-type-schema.json
slug: cognito-idp-resource-servers-list-type
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"UserPoolId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/UserPoolIdType\"\n          },\n          {\n            \"description\": \"The user pool ID for the user pool that hosts the resource server.\"\n          }\n        ]\n      },\n      \"Identifier\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceServerIdentifierType\"\n          },\n          {\n            \"description\": \"The identifier for the resource server.\"\n          }\n        ]\n      },\n      \"Name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceServerNameType\"\n          },\n          {\n            \"description\": \"The name of the resource server.\"\n          }\n        ]\n      },\n      \"Scopes\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceServerScopeListType\"\
  \n          },\n          {\n            \"description\": \"A list of scopes that are defined for the resource server.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A container for information about a resource server for a user pool.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-resource-servers-list-type-schema.json\",\n  \"title\": \"ResourceServersListType\",\n  \"description\": \"ResourceServersListType schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-resource-servers-list-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ResourceServersListType
---
