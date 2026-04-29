---
description: SetPrincipalTagAttributeMapResponse schema from Amazon Cognito API
layout: schema
name: SetPrincipalTagAttributeMapResponse
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
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-set-principal-tag-attribute-map-response-schema.json
slug: identity-pools-set-principal-tag-attribute-map-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-set-principal-tag-attribute-map-response-schema.json\",\n  \"title\": \"SetPrincipalTagAttributeMapResponse\",\n  \"description\": \"SetPrincipalTagAttributeMapResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"The ID of the Identity Pool you want to set attribute mappings for.\"\n        }\n      ]\n    },\n    \"IdentityProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderName\"\n        },\n        {\n          \"description\": \"The provider name you want to use for attribute mappings.\"\n        }\n      ]\n    },\n    \"\
  UseDefaults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UseDefaults\"\n        },\n        {\n          \"description\": \"You can use this operation to select default (username and clientID) attribute mappings.\"\n        }\n      ]\n    },\n    \"PrincipalTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrincipalTags\"\n        },\n        {\n          \"description\": \"You can use this operation to add principal tags. The <code>PrincipalTags</code>operation enables you to reference user attributes in your IAM permissions policy.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-set-principal-tag-attribute-map-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: SetPrincipalTagAttributeMapResponse
---
