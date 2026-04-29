---
description: Represents the response from the server to create a user pool client.
layout: schema
name: CreateUserPoolClientResponse
properties_list:
- description: ''
  name: UserPoolClient
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-create-user-pool-client-response-schema.json
slug: user-pools-create-user-pool-client-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-user-pool-client-response-schema.json\",\n  \"title\": \"CreateUserPoolClientResponse\",\n  \"description\": \"Represents the response from the server to create a user pool client.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolClient\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolClientType\"\n        },\n        {\n          \"description\": \"The user pool client that was just created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-user-pool-client-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: CreateUserPoolClientResponse
---
