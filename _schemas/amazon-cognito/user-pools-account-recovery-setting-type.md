---
description: The data type for <code>AccountRecoverySetting</code>.
layout: schema
name: AccountRecoverySettingType
properties_list:
- description: ''
  name: RecoveryMechanisms
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-account-recovery-setting-type-schema.json
slug: user-pools-account-recovery-setting-type
source_filename: user-pools-account-recovery-setting-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-account-recovery-setting-type-schema.json\",\n  \"title\": \"AccountRecoverySettingType\",\n  \"description\": \"The data type for <code>AccountRecoverySetting</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecoveryMechanisms\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecoveryMechanismsType\"\n        },\n        {\n          \"description\": \"The list of <code>RecoveryOptionTypes</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-account-recovery-setting-type-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: AccountRecoverySettingType
---
