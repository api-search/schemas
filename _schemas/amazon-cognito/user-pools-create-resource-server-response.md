---
description: CreateResourceServerResponse schema from Amazon Cognito API
layout: schema
name: CreateResourceServerResponse
properties_list:
- description: ''
  name: ResourceServer
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-create-resource-server-response-schema.json
slug: user-pools-create-resource-server-response
source_filename: user-pools-create-resource-server-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-resource-server-response-schema.json\",\n  \"title\": \"CreateResourceServerResponse\",\n  \"description\": \"CreateResourceServerResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceServer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceServerType\"\n        },\n        {\n          \"description\": \"The newly created resource server.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceServer\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-resource-server-response-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: CreateResourceServerResponse
---
