---
description: CreateIdentityProviderResponse schema from Amazon Cognito API
layout: schema
name: CreateIdentityProviderResponse
properties_list:
- description: ''
  name: IdentityProvider
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-create-identity-provider-response-schema.json
slug: user-pools-create-identity-provider-response
source_filename: user-pools-create-identity-provider-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-identity-provider-response-schema.json\",\n  \"title\": \"CreateIdentityProviderResponse\",\n  \"description\": \"CreateIdentityProviderResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityProviderType\"\n        },\n        {\n          \"description\": \"The newly created IdP object.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"IdentityProvider\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-create-identity-provider-response-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: CreateIdentityProviderResponse
---
