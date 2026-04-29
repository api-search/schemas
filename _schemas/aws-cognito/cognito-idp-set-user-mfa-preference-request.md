---
description: SetUserMFAPreferenceRequest schema from Amazon Cognito
layout: schema
name: SetUserMFAPreferenceRequest
properties_list:
- description: ''
  name: SMSMfaSettings
  type: object
- description: ''
  name: SoftwareTokenMfaSettings
  type: object
- description: ''
  name: AccessToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-set-user-mfa-preference-request-schema.json
slug: cognito-idp-set-user-mfa-preference-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SMSMfaSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SMSMfaSettingsType\"\n        },\n        {\n          \"description\": \"The SMS text message multi-factor authentication (MFA) settings.\"\n        }\n      ]\n    },\n    \"SoftwareTokenMfaSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SoftwareTokenMfaSettingsType\"\n        },\n        {\n          \"description\": \"The time-based one-time password (TOTP) software token MFA settings.\"\n        }\n      ]\n    },\n    \"AccessToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TokenModelType\"\n        },\n        {\n          \"description\": \"A valid access token that Amazon Cognito issued to the user whose MFA preference you want to set.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccessToken\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-set-user-mfa-preference-request-schema.json\",\n  \"title\": \"SetUserMFAPreferenceRequest\",\n  \"description\": \"SetUserMFAPreferenceRequest schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-set-user-mfa-preference-request-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: SetUserMFAPreferenceRequest
---
