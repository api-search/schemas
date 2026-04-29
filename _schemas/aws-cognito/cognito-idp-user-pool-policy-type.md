---
description: The policy associated with a user pool.
layout: schema
name: UserPoolPolicyType
properties_list:
- description: ''
  name: PasswordPolicy
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-user-pool-policy-type-schema.json
slug: cognito-idp-user-pool-policy-type
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"PasswordPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PasswordPolicyType\"\n        },\n        {\n          \"description\": \"The password policy.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The policy associated with a user pool.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-user-pool-policy-type-schema.json\",\n  \"title\": \"UserPoolPolicyType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-user-pool-policy-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: UserPoolPolicyType
---
