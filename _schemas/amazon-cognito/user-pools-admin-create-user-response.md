---
description: Represents the response from the server to the request to create the user.
layout: schema
name: AdminCreateUserResponse
properties_list:
- description: ''
  name: User
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-admin-create-user-response-schema.json
slug: user-pools-admin-create-user-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-create-user-response-schema.json\",\n  \"title\": \"AdminCreateUserResponse\",\n  \"description\": \"Represents the response from the server to the request to create the user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"User\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserType\"\n        },\n        {\n          \"description\": \"The newly created user.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-create-user-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: AdminCreateUserResponse
---
