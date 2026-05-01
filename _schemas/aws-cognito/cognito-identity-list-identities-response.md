---
description: The response to a ListIdentities request.
layout: schema
name: ListIdentitiesResponse
properties_list:
- description: ''
  name: IdentityPoolId
  type: object
- description: ''
  name: Identities
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-list-identities-response-schema.json
slug: cognito-identity-list-identities-response
source_filename: cognito-identity-list-identities-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"An identity pool ID in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"Identities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentitiesList\"\n        },\n        {\n          \"description\": \"An object containing a set of identities and associated mappings.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKey\"\n        },\n        {\n          \"description\": \"A pagination token.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The response to a ListIdentities request.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-list-identities-response-schema.json\"\
  ,\n  \"title\": \"ListIdentitiesResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-list-identities-response-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ListIdentitiesResponse
---
