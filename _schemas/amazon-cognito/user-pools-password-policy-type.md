---
description: The password policy type.
layout: schema
name: PasswordPolicyType
properties_list:
- description: ''
  name: MinimumLength
  type: object
- description: ''
  name: RequireUppercase
  type: object
- description: ''
  name: RequireLowercase
  type: object
- description: ''
  name: RequireNumbers
  type: object
- description: ''
  name: RequireSymbols
  type: object
- description: ''
  name: TemporaryPasswordValidityDays
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-password-policy-type-schema.json
slug: user-pools-password-policy-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-password-policy-type-schema.json\",\n  \"title\": \"PasswordPolicyType\",\n  \"description\": \"The password policy type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MinimumLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PasswordPolicyMinLengthType\"\n        },\n        {\n          \"description\": \"The minimum length of the password in the policy that you have set. This value can't be less than 6.\"\n        }\n      ]\n    },\n    \"RequireUppercase\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"In the password policy that you have set, refers to whether you have required users to use at least one uppercase letter in their password.\"\n  \
  \      }\n      ]\n    },\n    \"RequireLowercase\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"In the password policy that you have set, refers to whether you have required users to use at least one lowercase letter in their password.\"\n        }\n      ]\n    },\n    \"RequireNumbers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"In the password policy that you have set, refers to whether you have required users to use at least one number in their password.\"\n        }\n      ]\n    },\n    \"RequireSymbols\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"In the password policy that you have set, refers to whether you have required users to use at least one symbol in their password.\"\n \
  \       }\n      ]\n    },\n    \"TemporaryPasswordValidityDays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemporaryPasswordValidityDaysType\"\n        },\n        {\n          \"description\": \"<p>The number of days a temporary password is valid in the password policy. If the user doesn't sign in during this time, an administrator must reset their password.</p> <note> <p>When you set <code>TemporaryPasswordValidityDays</code> for a user pool, you can no longer set a value for the legacy <code>UnusedAccountValidityDays</code> parameter in that user pool.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-password-policy-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: PasswordPolicyType
---
