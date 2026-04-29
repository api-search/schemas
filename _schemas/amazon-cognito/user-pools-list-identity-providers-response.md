---
description: ListIdentityProvidersResponse schema from Amazon Cognito API
layout: schema
name: ListIdentityProvidersResponse
properties_list:
- description: ''
  name: Providers
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-list-identity-providers-response-schema.json
slug: user-pools-list-identity-providers-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-identity-providers-response-schema.json\",\n  \"title\": \"ListIdentityProvidersResponse\",\n  \"description\": \"ListIdentityProvidersResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Providers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvidersListType\"\n        },\n        {\n          \"description\": \"A list of IdP objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKeyType\"\n        },\n        {\n          \"description\": \"A pagination token.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Providers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-list-identity-providers-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: ListIdentityProvidersResponse
---
