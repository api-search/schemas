---
description: ListIdentityProvidersRequest schema from Amazon Cognito API
layout: schema
name: ListIdentityProvidersRequest
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
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-list-identity-providers-request-schema.json
slug: user-pools-list-identity-providers-request
source_filename: user-pools-list-identity-providers-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-identity-providers-request-schema.json\",\n  \"title\": \"ListIdentityProvidersRequest\",\n  \"description\": \"ListIdentityProvidersRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListProvidersLimitType\"\n        },\n        {\n          \"description\": \"The maximum number of IdPs to return.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKeyType\"\n\
  \        },\n        {\n          \"description\": \"A pagination token.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-identity-providers-request-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: ListIdentityProvidersRequest
---
