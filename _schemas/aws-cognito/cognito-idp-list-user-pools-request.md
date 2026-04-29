---
description: Represents the request to list user pools.
layout: schema
name: ListUserPoolsRequest
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-list-user-pools-request-schema.json
slug: cognito-idp-list-user-pools-request
source_filename: cognito-idp-list-user-pools-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKeyType\"\n        },\n        {\n          \"description\": \"An identifier that was returned from the previous call to this operation, which can be used to return the next set of items in the list.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolQueryLimitType\"\n        },\n        {\n          \"description\": \"The maximum number of results you want the request to return when listing the user pools.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MaxResults\"\n  ],\n  \"description\": \"Represents the request to list user pools.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-user-pools-request-schema.json\"\
  ,\n  \"title\": \"ListUserPoolsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-list-user-pools-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ListUserPoolsRequest
---
