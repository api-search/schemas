---
description: CreateResourceServerRequest schema from Amazon Cognito
layout: schema
name: CreateResourceServerRequest
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
schema_file: json-schema/cognito-idp-create-resource-server-request-schema.json
slug: cognito-idp-create-resource-server-request
source_filename: cognito-idp-create-resource-server-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool.\"\n        }\n      ]\n    },\n    \"Identifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerIdentifierType\"\n        },\n        {\n          \"description\": \"A unique resource server identifier for the resource server. This could be an HTTPS endpoint where the resource server is located, such as <code>https://my-weather-api.example.com</code>.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerNameType\"\n        },\n        {\n          \"description\": \"A friendly name for the resource server.\"\n        }\n      ]\n    },\n    \"Scopes\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/ResourceServerScopeListType\"\n        },\n        {\n          \"description\": \"A list of scopes. Each scope is a key-value map with the keys <code>name</code> and <code>description</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"Identifier\",\n    \"Name\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-create-resource-server-request-schema.json\",\n  \"title\": \"CreateResourceServerRequest\",\n  \"description\": \"CreateResourceServerRequest schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-create-resource-server-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: CreateResourceServerRequest
---
