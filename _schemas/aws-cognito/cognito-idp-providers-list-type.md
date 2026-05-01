---
description: ProvidersListType schema from Amazon Cognito
layout: schema
name: ProvidersListType
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-providers-list-type-schema.json
slug: cognito-idp-providers-list-type
source_filename: cognito-idp-providers-list-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"ProviderName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ProviderNameType\"\n          },\n          {\n            \"description\": \"The IdP name.\"\n          }\n        ]\n      },\n      \"ProviderType\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IdentityProviderTypeType\"\n          },\n          {\n            \"description\": \"The IdP type.\"\n          }\n        ]\n      },\n      \"LastModifiedDate\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DateType\"\n          },\n          {\n            \"description\": \"The date the provider was last modified.\"\n          }\n        ]\n      },\n      \"CreationDate\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DateType\"\n          },\n          {\n         \
  \   \"description\": \"The date the provider was added to the user pool.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A container for IdP details.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-providers-list-type-schema.json\",\n  \"title\": \"ProvidersListType\",\n  \"description\": \"ProvidersListType schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-providers-list-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ProvidersListType
---
