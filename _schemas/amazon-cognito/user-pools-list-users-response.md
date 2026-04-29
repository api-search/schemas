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
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-list-users-response-schema.json
slug: user-pools-list-users-response
source_filename: user-pools-list-users-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-users-response-schema.json\",\n  \"title\": \"ListUsersResponse\",\n  \"description\": \"The response from the request to list users.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Users\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsersListType\"\n        },\n        {\n          \"description\": \"<p>A list of the user pool users, and their attributes, that match your query.</p> <note> <p>Amazon Cognito creates a profile in your user pool for each native user in your user pool, and each unique user ID from your third-party identity providers (IdPs). When you link users with the <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_AdminLinkProviderForUser.html\\\">AdminLinkProviderForUser</a> API operation,\
  \ the output of <code>ListUsers</code> displays both the IdP user and the native user that you linked. You can identify IdP users in the <code>Users</code> object of this API response by the IdP prefix that Amazon Cognito appends to <code>Username</code>.</p> </note>\"\n        }\n      ]\n    },\n    \"PaginationToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SearchPaginationTokenType\"\n        },\n        {\n          \"description\": \"An identifier that was returned from the previous call to this operation, which can be used to return the next set of items in the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-users-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: ListUsersResponse
---
