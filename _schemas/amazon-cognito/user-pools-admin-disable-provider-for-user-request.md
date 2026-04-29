---
description: AdminDisableProviderForUserRequest schema from Amazon Cognito API
layout: schema
name: AdminDisableProviderForUserRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: User
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-admin-disable-provider-for-user-request-schema.json
slug: user-pools-admin-disable-provider-for-user-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-disable-provider-for-user-request-schema.json\",\n  \"title\": \"AdminDisableProviderForUserRequest\",\n  \"description\": \"AdminDisableProviderForUserRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The user pool ID for the user pool.\"\n        }\n      ]\n    },\n    \"User\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProviderUserIdentifierType\"\n        },\n        {\n          \"description\": \"The user to be disabled.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\",\n    \"User\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-admin-disable-provider-for-user-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: AdminDisableProviderForUserRequest
---
