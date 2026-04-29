---
description: <i>This data type is no longer supported.</i> Applies only to SMS multi-factor authentication (MFA) configurations. Does not apply to time-based one-time password (TOTP) software token MFA configurations.
layout: schema
name: MFAOptionType
properties_list:
- description: ''
  name: DeliveryMedium
  type: object
- description: ''
  name: AttributeName
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-mfa-option-type-schema.json
slug: user-pools-mfa-option-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-mfa-option-type-schema.json\",\n  \"title\": \"MFAOptionType\",\n  \"description\": \" <i>This data type is no longer supported.</i> Applies only to SMS multi-factor authentication (MFA) configurations. Does not apply to time-based one-time password (TOTP) software token MFA configurations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeliveryMedium\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryMediumType\"\n        },\n        {\n          \"description\": \"The delivery medium to send the MFA code. You can use this parameter to set only the <code>SMS</code> delivery medium value.\"\n        }\n      ]\n    },\n    \"AttributeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeNameType\"\n        },\n\
  \        {\n          \"description\": \"The attribute name of the MFA option type. The only valid value is <code>phone_number</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-mfa-option-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: MFAOptionType
---
