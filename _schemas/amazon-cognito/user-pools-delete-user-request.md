---
description: Represents the request to delete a user.
layout: schema
name: DeleteUserRequest
properties_list:
- description: ''
  name: AccessToken
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-delete-user-request-schema.json
slug: user-pools-delete-user-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-delete-user-request-schema.json\",\n  \"title\": \"DeleteUserRequest\",\n  \"description\": \"Represents the request to delete a user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user whose user profile you want to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccessToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-delete-user-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: DeleteUserRequest
---
