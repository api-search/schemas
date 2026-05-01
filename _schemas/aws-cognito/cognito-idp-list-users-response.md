---
description: The response from the request to list users.
layout: schema
name: ListUsersResponse
properties_list:
- description: ''
  name: Users
  type: object
- description: ''
  name: PaginationToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-list-users-response-schema.json
slug: cognito-idp-list-users-response
source_filename: cognito-idp-list-users-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Users\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsersListType\"\n        },\n        {\n          \"description\": \"The users returned in the request to list users.\"\n        }\n      ]\n    },\n    \"PaginationToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchPaginationTokenType\"\n        },\n        {\n          \"description\": \"An identifier that was returned from the previous call to this operation, which can be used to return the next set of items in the list.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The response from the request to list users.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-users-response-schema.json\",\n  \"title\": \"ListUsersResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-users-response-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ListUsersResponse
---
