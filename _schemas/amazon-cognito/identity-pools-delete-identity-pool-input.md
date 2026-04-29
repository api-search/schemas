---
description: Input to the DeleteIdentityPool action.
layout: schema
name: DeleteIdentityPoolInput
properties_list:
- description: ''
  name: IdentityPoolId
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/identity-pools-delete-identity-pool-input-schema.json
slug: identity-pools-delete-identity-pool-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-delete-identity-pool-input-schema.json\",\n  \"title\": \"DeleteIdentityPoolInput\",\n  \"description\": \"Input to the DeleteIdentityPool action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityPoolId\"\n        },\n        {\n          \"description\": \"An identity pool ID in the format REGION:GUID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityPoolId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/identity-pools-delete-identity-pool-input-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: DeleteIdentityPoolInput
---
