---
description: Represents the request to list the user pool clients.
layout: schema
name: ListUserPoolClientsRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-list-user-pool-clients-request-schema.json
slug: cognito-idp-list-user-pool-clients-request
source_filename: cognito-idp-list-user-pool-clients-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool where you want to list user pool clients.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryLimit\"\n        },\n        {\n          \"description\": \"The maximum number of results you want the request to return when listing the user pool clients.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKey\"\n        },\n        {\n          \"description\": \"An identifier that was returned from the previous call to this operation, which can be used to return the next set of items in the list.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\"\
  \n  ],\n  \"description\": \"Represents the request to list the user pool clients.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-user-pool-clients-request-schema.json\",\n  \"title\": \"ListUserPoolClientsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-user-pool-clients-request-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ListUserPoolClientsRequest
---
