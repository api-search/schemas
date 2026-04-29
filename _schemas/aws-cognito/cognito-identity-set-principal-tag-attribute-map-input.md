---
description: SetPrincipalTagAttributeMapInput schema from Amazon Cognito
layout: schema
name: SetPrincipalTagAttributeMapInput
properties_list:
- description: ''
  name: IdentityPoolId
  type: object
- description: ''
  name: IdentityProviderName
  type: object
- description: ''
  name: UseDefaults
  type: object
- description: ''
  name: PrincipalTags
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-set-principal-tag-attribute-map-input-schema.json
slug: cognito-identity-set-principal-tag-attribute-map-input
source_filename: cognito-identity-set-principal-tag-attribute-map-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"The ID of the Identity Pool you want to set attribute mappings for.\"\n        }\n      ]\n    },\n    \"IdentityProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderName\"\n        },\n        {\n          \"description\": \"The provider name you want to use for attribute mappings.\"\n        }\n      ]\n    },\n    \"UseDefaults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UseDefaults\"\n        },\n        {\n          \"description\": \"You can use this operation to use default (username and clientID) attribute mappings.\"\n        }\n      ]\n    },\n    \"PrincipalTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrincipalTags\"\
  \n        },\n        {\n          \"description\": \"You can use this operation to add principal tags.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityPoolId\",\n    \"IdentityProviderName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-set-principal-tag-attribute-map-input-schema.json\",\n  \"title\": \"SetPrincipalTagAttributeMapInput\",\n  \"description\": \"SetPrincipalTagAttributeMapInput schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-set-principal-tag-attribute-map-input-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: SetPrincipalTagAttributeMapInput
---
