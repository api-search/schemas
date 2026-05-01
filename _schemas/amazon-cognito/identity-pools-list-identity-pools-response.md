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
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-list-identity-pools-response-schema.json
slug: identity-pools-list-identity-pools-response
source_filename: identity-pools-list-identity-pools-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-list-identity-pools-response-schema.json\",\n  \"title\": \"ListIdentityPoolsResponse\",\n  \"description\": \"The result of a successful ListIdentityPools action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPools\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolsList\"\n        },\n        {\n          \"description\": \"The identity pools returned by the ListIdentityPools action.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKey\"\n        },\n        {\n          \"description\": \"A pagination token.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-list-identity-pools-response-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: ListIdentityPoolsResponse
---
