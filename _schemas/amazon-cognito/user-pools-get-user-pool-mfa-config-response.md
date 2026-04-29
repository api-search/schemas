---
description: GetUserPoolMfaConfigResponse schema from Amazon Cognito API
layout: schema
name: GetUserPoolMfaConfigResponse
properties_list:
- description: ''
  name: SmsMfaConfiguration
  type: object
- description: ''
  name: SoftwareTokenMfaConfiguration
  type: object
- description: ''
  name: MfaConfiguration
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-get-user-pool-mfa-config-response-schema.json
slug: user-pools-get-user-pool-mfa-config-response
source_filename: user-pools-get-user-pool-mfa-config-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-user-pool-mfa-config-response-schema.json\",\n  \"title\": \"GetUserPoolMfaConfigResponse\",\n  \"description\": \"GetUserPoolMfaConfigResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SmsMfaConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsMfaConfigType\"\n        },\n        {\n          \"description\": \"The SMS text message multi-factor authentication (MFA) configuration.\"\n        }\n      ]\n    },\n    \"SoftwareTokenMfaConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SoftwareTokenMfaConfigType\"\n        },\n        {\n          \"description\": \"The software token multi-factor authentication (MFA) configuration.\"\n        }\n      ]\n    },\n\
  \    \"MfaConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolMfaType\"\n        },\n        {\n          \"description\": \"<p>The multi-factor authentication (MFA) configuration. Valid values include:</p> <ul> <li> <p> <code>OFF</code> MFA won't be used for any users.</p> </li> <li> <p> <code>ON</code> MFA is required for all users to sign in.</p> </li> <li> <p> <code>OPTIONAL</code> MFA will be required only for individual users who have an MFA factor activated.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-user-pool-mfa-config-response-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: GetUserPoolMfaConfigResponse
---
