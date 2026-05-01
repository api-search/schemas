---
description: The data type for <code>AccountRecoverySetting</code>.
layout: schema
name: AccountRecoverySettingType
properties_list:
- description: ''
  name: RecoveryMechanisms
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-account-recovery-setting-type-schema.json
slug: cognito-idp-account-recovery-setting-type
source_filename: cognito-idp-account-recovery-setting-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecoveryMechanisms\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecoveryMechanismsType\"\n        },\n        {\n          \"description\": \"The list of <code>RecoveryOptionTypes</code>.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The data type for <code>AccountRecoverySetting</code>.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-account-recovery-setting-type-schema.json\",\n  \"title\": \"AccountRecoverySettingType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-account-recovery-setting-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AccountRecoverySettingType
---
