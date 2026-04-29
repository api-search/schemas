---
description: The type used for enabling software token MFA at the user pool level.
layout: schema
name: SoftwareTokenMfaConfigType
properties_list:
- description: ''
  name: Enabled
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-software-token-mfa-config-type-schema.json
slug: user-pools-software-token-mfa-config-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-software-token-mfa-config-type-schema.json\",\n  \"title\": \"SoftwareTokenMfaConfigType\",\n  \"description\": \"The type used for enabling software token MFA at the user pool level.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"Specifies whether software token MFA is activated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-software-token-mfa-config-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: SoftwareTokenMfaConfigType
---
