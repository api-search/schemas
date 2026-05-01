---
description: Input to the ListIdentities action.
layout: schema
name: ListIdentitiesInput
properties_list:
- description: ''
  name: IdentityPoolId
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: HideDisabled
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-list-identities-input-schema.json
slug: cognito-identity-list-identities-input
source_filename: cognito-identity-list-identities-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"An identity pool ID in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryLimit\"\n        },\n        {\n          \"description\": \"The maximum number of identities to return.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKey\"\n        },\n        {\n          \"description\": \"A pagination token.\"\n        }\n      ]\n    },\n    \"HideDisabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HideDisabled\"\n        },\n        {\n          \"description\": \"An optional boolean parameter that allows you to hide disabled identities.\
  \ If omitted, the ListIdentities API will include disabled identities in the response.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityPoolId\",\n    \"MaxResults\"\n  ],\n  \"description\": \"Input to the ListIdentities action.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-list-identities-input-schema.json\",\n  \"title\": \"ListIdentitiesInput\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-list-identities-input-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ListIdentitiesInput
---
