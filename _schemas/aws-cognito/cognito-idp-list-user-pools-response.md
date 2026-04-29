---
description: Represents the response to list user pools.
layout: schema
name: ListUserPoolsResponse
properties_list:
- description: ''
  name: UserPools
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-list-user-pools-response-schema.json
slug: cognito-idp-list-user-pools-response
source_filename: cognito-idp-list-user-pools-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPools\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolListType\"\n        },\n        {\n          \"description\": \"The user pools from the response to list users.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKeyType\"\n        },\n        {\n          \"description\": \"An identifier that was returned from the previous call to this operation, which can be used to return the next set of items in the list.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Represents the response to list user pools.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-user-pools-response-schema.json\",\n  \"title\": \"ListUserPoolsResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-user-pools-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ListUserPoolsResponse
---
