---
description: Represents the request to get information about the user.
layout: schema
name: GetUserRequest
properties_list:
- description: ''
  name: AccessToken
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-get-user-request-schema.json
slug: user-pools-get-user-request
source_filename: user-pools-get-user-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-user-request-schema.json\",\n  \"title\": \"GetUserRequest\",\n  \"description\": \"Represents the request to get information about the user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A non-expired access token for the user whose information you want to query.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccessToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-user-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: GetUserRequest
---
