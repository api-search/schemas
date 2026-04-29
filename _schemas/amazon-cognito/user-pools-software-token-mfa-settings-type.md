---
description: The type used for enabling software token MFA at the user level. If an MFA type is activated for a user, the user will be prompted for MFA during all sign-in attempts, unless device tracking is turned on and the device has been trusted. If you want MFA to be applied selectively based on the assessed risk level of sign-in attempts, deactivate MFA for users and turn on Adaptive Authentication for the user pool.
layout: schema
name: SoftwareTokenMfaSettingsType
properties_list:
- description: ''
  name: Enabled
  type: object
- description: ''
  name: PreferredMfa
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-software-token-mfa-settings-type-schema.json
slug: user-pools-software-token-mfa-settings-type
source_filename: user-pools-software-token-mfa-settings-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-software-token-mfa-settings-type-schema.json\",\n  \"title\": \"SoftwareTokenMfaSettingsType\",\n  \"description\": \"The type used for enabling software token MFA at the user level. If an MFA type is activated for a user, the user will be prompted for MFA during all sign-in attempts, unless device tracking is turned on and the device has been trusted. If you want MFA to be applied selectively based on the assessed risk level of sign-in attempts, deactivate MFA for users and turn on Adaptive Authentication for the user pool.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"Specifies whether software token MFA is activated. If an MFA\
  \ type is activated for a user, the user will be prompted for MFA during all sign-in attempts, unless device tracking is turned on and the device has been trusted.\"\n        }\n      ]\n    },\n    \"PreferredMfa\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"Specifies whether software token MFA is the preferred MFA method.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-software-token-mfa-settings-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: SoftwareTokenMfaSettingsType
---
