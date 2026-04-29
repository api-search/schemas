---
description: UpdateResourceServerRequest schema from Amazon Cognito
layout: schema
name: UpdateResourceServerRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: Identifier
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Scopes
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-update-resource-server-request-schema.json
slug: cognito-idp-update-resource-server-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool.\"\n        }\n      ]\n    },\n    \"Identifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerIdentifierType\"\n        },\n        {\n          \"description\": \"The identifier for the resource server.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerNameType\"\n        },\n        {\n          \"description\": \"The name of the resource server.\"\n        }\n      ]\n    },\n    \"Scopes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerScopeListType\"\n        },\n        {\n          \"description\": \"The scope values to be set for the resource\
  \ server.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"Identifier\",\n    \"Name\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-update-resource-server-request-schema.json\",\n  \"title\": \"UpdateResourceServerRequest\",\n  \"description\": \"UpdateResourceServerRequest schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-update-resource-server-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UpdateResourceServerRequest
---
