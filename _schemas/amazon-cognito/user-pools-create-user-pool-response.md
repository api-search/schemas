---
description: Represents the response from the server for the request to create a user pool.
layout: schema
name: CreateUserPoolResponse
properties_list:
- description: ''
  name: UserPool
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-create-user-pool-response-schema.json
slug: user-pools-create-user-pool-response
source_filename: user-pools-create-user-pool-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-user-pool-response-schema.json\",\n  \"title\": \"CreateUserPoolResponse\",\n  \"description\": \"Represents the response from the server for the request to create a user pool.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPool\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolType\"\n        },\n        {\n          \"description\": \"A container for the user pool details.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-user-pool-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: CreateUserPoolResponse
---
