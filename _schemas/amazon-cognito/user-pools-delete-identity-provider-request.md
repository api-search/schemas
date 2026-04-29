---
description: DeleteIdentityProviderRequest schema from Amazon Cognito API
layout: schema
name: DeleteIdentityProviderRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: ProviderName
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-delete-identity-provider-request-schema.json
slug: user-pools-delete-identity-provider-request
source_filename: user-pools-delete-identity-provider-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-delete-identity-provider-request-schema.json\",\n  \"title\": \"DeleteIdentityProviderRequest\",\n  \"description\": \"DeleteIdentityProviderRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"ProviderName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProviderNameType\"\n        },\n        {\n          \"description\": \"The IdP name.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"ProviderName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-delete-identity-provider-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: DeleteIdentityProviderRequest
---
