---
description: GetUserPoolMfaConfigRequest schema from Amazon Cognito API
layout: schema
name: GetUserPoolMfaConfigRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-get-user-pool-mfa-config-request-schema.json
slug: user-pools-get-user-pool-mfa-config-request
source_filename: user-pools-get-user-pool-mfa-config-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-user-pool-mfa-config-request-schema.json\",\n  \"title\": \"GetUserPoolMfaConfigRequest\",\n  \"description\": \"GetUserPoolMfaConfigRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-user-pool-mfa-config-request-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: GetUserPoolMfaConfigRequest
---
