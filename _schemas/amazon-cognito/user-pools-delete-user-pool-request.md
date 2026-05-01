---
description: Represents the request to delete a user pool.
layout: schema
name: DeleteUserPoolRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-delete-user-pool-request-schema.json
slug: user-pools-delete-user-pool-request
source_filename: user-pools-delete-user-pool-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-delete-user-pool-request-schema.json\",\n  \"title\": \"DeleteUserPoolRequest\",\n  \"description\": \"Represents the request to delete a user pool.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool you want to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-delete-user-pool-request-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: DeleteUserPoolRequest
---
