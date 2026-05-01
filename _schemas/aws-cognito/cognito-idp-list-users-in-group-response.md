---
description: ListUsersInGroupResponse schema from Amazon Cognito
layout: schema
name: ListUsersInGroupResponse
properties_list:
- description: ''
  name: Users
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-list-users-in-group-response-schema.json
slug: cognito-idp-list-users-in-group-response
source_filename: cognito-idp-list-users-in-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Users\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsersListType\"\n        },\n        {\n          \"description\": \"The users returned in the request to list users.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKey\"\n        },\n        {\n          \"description\": \"An identifier that you can use in a later request to return the next set of items in the list.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-users-in-group-response-schema.json\",\n  \"title\": \"ListUsersInGroupResponse\",\n  \"description\": \"ListUsersInGroupResponse schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-users-in-group-response-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ListUsersInGroupResponse
---
