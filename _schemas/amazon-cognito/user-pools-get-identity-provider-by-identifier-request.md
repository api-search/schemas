---
description: GetIdentityProviderByIdentifierRequest schema from Amazon Cognito API
layout: schema
name: GetIdentityProviderByIdentifierRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: IdpIdentifier
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-get-identity-provider-by-identifier-request-schema.json
slug: user-pools-get-identity-provider-by-identifier-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-identity-provider-by-identifier-request-schema.json\",\n  \"title\": \"GetIdentityProviderByIdentifierRequest\",\n  \"description\": \"GetIdentityProviderByIdentifierRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"IdpIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdpIdentifierType\"\n        },\n        {\n          \"description\": \"The IdP identifier.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"IdpIdentifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-identity-provider-by-identifier-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: GetIdentityProviderByIdentifierRequest
---
