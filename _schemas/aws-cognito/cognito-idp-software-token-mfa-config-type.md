---
description: The type used for enabling software token MFA at the user pool level.
layout: schema
name: SoftwareTokenMfaConfigType
properties_list:
- description: ''
  name: Enabled
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-software-token-mfa-config-type-schema.json
slug: cognito-idp-software-token-mfa-config-type
source_filename: cognito-idp-software-token-mfa-config-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"Specifies whether software token MFA is activated.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The type used for enabling software token MFA at the user pool level.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-software-token-mfa-config-type-schema.json\",\n  \"title\": \"SoftwareTokenMfaConfigType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-software-token-mfa-config-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: SoftwareTokenMfaConfigType
---
