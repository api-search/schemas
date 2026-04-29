---
description: A resource server scope.
layout: schema
name: ResourceServerScopeType
properties_list:
- description: ''
  name: ScopeName
  type: object
- description: ''
  name: ScopeDescription
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-resource-server-scope-type-schema.json
slug: cognito-idp-resource-server-scope-type
source_filename: cognito-idp-resource-server-scope-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScopeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerScopeNameType\"\n        },\n        {\n          \"description\": \"The name of the scope.\"\n        }\n      ]\n    },\n    \"ScopeDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerScopeDescriptionType\"\n        },\n        {\n          \"description\": \"A description of the scope.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ScopeName\",\n    \"ScopeDescription\"\n  ],\n  \"description\": \"A resource server scope.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-resource-server-scope-type-schema.json\",\n  \"title\": \"ResourceServerScopeType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-resource-server-scope-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ResourceServerScopeType
---
