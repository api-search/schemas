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
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-list-identities-response-schema.json
slug: identity-pools-list-identities-response
source_filename: identity-pools-list-identities-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-list-identities-response-schema.json\",\n  \"title\": \"ListIdentitiesResponse\",\n  \"description\": \"The response to a ListIdentities request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"An identity pool ID in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"Identities\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentitiesList\"\n        },\n        {\n          \"description\": \"An object containing a set of identities and associated mappings.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKey\"\
  \n        },\n        {\n          \"description\": \"A pagination token.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-list-identities-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: ListIdentitiesResponse
---
