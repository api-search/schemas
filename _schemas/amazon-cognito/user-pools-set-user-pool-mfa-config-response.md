---
description: SetUserPoolMfaConfigResponse schema from Amazon Cognito API
layout: schema
name: SetUserPoolMfaConfigResponse
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
schema_file: json-schema/user-pools-set-user-pool-mfa-config-response-schema.json
slug: user-pools-set-user-pool-mfa-config-response
source_filename: user-pools-set-user-pool-mfa-config-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-set-user-pool-mfa-config-response-schema.json\",\n  \"title\": \"SetUserPoolMfaConfigResponse\",\n  \"description\": \"SetUserPoolMfaConfigResponse schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SmsMfaConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsMfaConfigType\"\n        },\n        {\n          \"description\": \"The SMS text message MFA configuration.\"\n        }\n      ]\n    },\n    \"SoftwareTokenMfaConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SoftwareTokenMfaConfigType\"\n        },\n        {\n          \"description\": \"The software token MFA configuration.\"\n        }\n      ]\n    },\n    \"MfaConfiguration\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/UserPoolMfaType\"\n        },\n        {\n          \"description\": \"<p>The MFA configuration. Valid values include:</p> <ul> <li> <p> <code>OFF</code> MFA won't be used for any users.</p> </li> <li> <p> <code>ON</code> MFA is required for all users to sign in.</p> </li> <li> <p> <code>OPTIONAL</code> MFA will be required only for individual users who have an MFA factor enabled.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-set-user-pool-mfa-config-response-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: SetUserPoolMfaConfigResponse
---
