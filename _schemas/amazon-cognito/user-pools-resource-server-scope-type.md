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
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-resource-server-scope-type-schema.json
slug: user-pools-resource-server-scope-type
source_filename: user-pools-resource-server-scope-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-resource-server-scope-type-schema.json\",\n  \"title\": \"ResourceServerScopeType\",\n  \"description\": \"A resource server scope.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScopeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerScopeNameType\"\n        },\n        {\n          \"description\": \"The name of the scope.\"\n        }\n      ]\n    },\n    \"ScopeDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerScopeDescriptionType\"\n        },\n        {\n          \"description\": \"A description of the scope.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ScopeName\",\n    \"ScopeDescription\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-resource-server-scope-type-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: ResourceServerScopeType
---
