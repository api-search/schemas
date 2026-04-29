---
description: The result of a successful ListIdentityPools action.
layout: schema
name: ListIdentityPoolsResponse
properties_list:
- description: ''
  name: IdentityPools
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-list-identity-pools-response-schema.json
slug: cognito-identity-list-identity-pools-response
source_filename: cognito-identity-list-identity-pools-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPools\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolsList\"\n        },\n        {\n          \"description\": \"The identity pools returned by the ListIdentityPools action.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKey\"\n        },\n        {\n          \"description\": \"A pagination token.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The result of a successful ListIdentityPools action.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-list-identity-pools-response-schema.json\",\n  \"title\": \"ListIdentityPoolsResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-list-identity-pools-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ListIdentityPoolsResponse
---
