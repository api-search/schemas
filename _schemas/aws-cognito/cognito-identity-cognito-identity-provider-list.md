---
description: CognitoIdentityProviderList schema from Amazon Cognito
layout: schema
name: CognitoIdentityProviderList
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-cognito-identity-provider-list-schema.json
slug: cognito-identity-cognito-identity-provider-list
source_filename: cognito-identity-cognito-identity-provider-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"ProviderName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/CognitoIdentityProviderName\"\n          },\n          {\n            \"description\": \"The provider name for an Amazon Cognito user pool. For example, <code>cognito-idp.us-east-1.amazonaws.com/us-east-1_123456789</code>.\"\n          }\n        ]\n      },\n      \"ClientId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/CognitoIdentityProviderClientId\"\n          },\n          {\n            \"description\": \"The client ID for the Amazon Cognito user pool.\"\n          }\n        ]\n      },\n      \"ServerSideTokenCheck\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/CognitoIdentityProviderTokenCheck\"\n          },\n          {\n            \"description\": \"<p>TRUE if server-side token validation\
  \ is enabled for the identity provider\\u2019s token.</p> <p>Once you set <code>ServerSideTokenCheck</code> to TRUE for an identity pool, that identity pool will check with the integrated user pools to make sure that the user has not been globally signed out or deleted before the identity pool provides an OIDC token or AWS credentials for the user.</p> <p>If the user is signed out or deleted, the identity pool will return a 400 Not Authorized error.</p>\"\n          }\n        ]\n      }\n    },\n    \"description\": \"A provider representing an Amazon Cognito user pool and its client ID.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-cognito-identity-provider-list-schema.json\",\n  \"title\": \"CognitoIdentityProviderList\",\n  \"description\": \"CognitoIdentityProviderList schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-cognito-identity-provider-list-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: CognitoIdentityProviderList
---
