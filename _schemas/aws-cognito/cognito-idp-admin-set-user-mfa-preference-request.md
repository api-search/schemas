---
description: AdminSetUserMFAPreferenceRequest schema from Amazon Cognito
layout: schema
name: AdminSetUserMFAPreferenceRequest
properties_list:
- description: ''
  name: SMSMfaSettings
  type: object
- description: ''
  name: SoftwareTokenMfaSettings
  type: object
- description: ''
  name: Username
  type: object
- description: ''
  name: UserPoolId
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-admin-set-user-mfa-preference-request-schema.json
slug: cognito-idp-admin-set-user-mfa-preference-request
source_filename: cognito-idp-admin-set-user-mfa-preference-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SMSMfaSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SMSMfaSettingsType\"\n        },\n        {\n          \"description\": \"The SMS text message MFA settings.\"\n        }\n      ]\n    },\n    \"SoftwareTokenMfaSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SoftwareTokenMfaSettingsType\"\n        },\n        {\n          \"description\": \"The time-based one-time password software token MFA settings.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UsernameType\"\n        },\n        {\n          \"description\": \"The user pool username or alias.\"\n        }\n      ]\n    },\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Username\",\n    \"UserPoolId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-set-user-mfa-preference-request-schema.json\",\n  \"title\": \"AdminSetUserMFAPreferenceRequest\",\n  \"description\": \"AdminSetUserMFAPreferenceRequest schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-admin-set-user-mfa-preference-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: AdminSetUserMFAPreferenceRequest
---
