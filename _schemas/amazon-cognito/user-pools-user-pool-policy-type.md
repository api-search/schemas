---
description: The policy associated with a user pool.
layout: schema
name: UserPoolPolicyType
properties_list:
- description: ''
  name: PasswordPolicy
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-user-pool-policy-type-schema.json
slug: user-pools-user-pool-policy-type
source_filename: user-pools-user-pool-policy-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-user-pool-policy-type-schema.json\",\n  \"title\": \"UserPoolPolicyType\",\n  \"description\": \"The policy associated with a user pool.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PasswordPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PasswordPolicyType\"\n        },\n        {\n          \"description\": \"The password policy.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-user-pool-policy-type-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: UserPoolPolicyType
---
