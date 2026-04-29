---
description: GetIdentityProviderByIdentifierResponse schema from Amazon Cognito API
layout: schema
name: GetIdentityProviderByIdentifierResponse
properties_list:
- description: ''
  name: IdentityProvider
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-get-identity-provider-by-identifier-response-schema.json
slug: user-pools-get-identity-provider-by-identifier-response
source_filename: user-pools-get-identity-provider-by-identifier-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-identity-provider-by-identifier-response-schema.json\",\n  \"title\": \"GetIdentityProviderByIdentifierResponse\",\n  \"description\": \"GetIdentityProviderByIdentifierResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderType\"\n        },\n        {\n          \"description\": \"The identity provider details.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityProvider\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-identity-provider-by-identifier-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: GetIdentityProviderByIdentifierResponse
---
