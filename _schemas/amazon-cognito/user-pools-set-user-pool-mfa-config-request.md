---
description: SetUserPoolMfaConfigRequest schema from Amazon Cognito API
layout: schema
name: SetUserPoolMfaConfigRequest
properties_list:
- description: ''
  name: UserPoolId
  type: object
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
schema_file: json-schema/user-pools-set-user-pool-mfa-config-request-schema.json
slug: user-pools-set-user-pool-mfa-config-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-set-user-pool-mfa-config-request-schema.json\",\n  \"title\": \"SetUserPoolMfaConfigRequest\",\n  \"description\": \"SetUserPoolMfaConfigRequest schema from Amazon Cognito API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"SmsMfaConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsMfaConfigType\"\n        },\n        {\n          \"description\": \"The SMS text message MFA configuration.\"\n        }\n      ]\n    },\n    \"SoftwareTokenMfaConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SoftwareTokenMfaConfigType\"\
  \n        },\n        {\n          \"description\": \"The software token MFA configuration.\"\n        }\n      ]\n    },\n    \"MfaConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolMfaType\"\n        },\n        {\n          \"description\": \"<p>The MFA configuration. If you set the MfaConfiguration value to \\u2018ON\\u2019, only users who have set up an MFA factor can sign in. To learn more, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/user-pool-settings-mfa.html\\\">Adding Multi-Factor Authentication (MFA) to a user pool</a>. Valid values include:</p> <ul> <li> <p> <code>OFF</code> MFA won't be used for any users.</p> </li> <li> <p> <code>ON</code> MFA is required for all users to sign in.</p> </li> <li> <p> <code>OPTIONAL</code> MFA will be required only for individual users who have an MFA factor activated.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"UserPoolId\"\n \
  \ ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-set-user-pool-mfa-config-request-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: SetUserPoolMfaConfigRequest
---
