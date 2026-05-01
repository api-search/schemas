---
description: The SMS text message multi-factor authentication (MFA) configuration type.
layout: schema
name: SmsMfaConfigType
properties_list:
- description: ''
  name: SmsAuthenticationMessage
  type: object
- description: ''
  name: SmsConfiguration
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-sms-mfa-config-type-schema.json
slug: cognito-idp-sms-mfa-config-type
source_filename: cognito-idp-sms-mfa-config-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SmsAuthenticationMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsVerificationMessageType\"\n        },\n        {\n          \"description\": \"The SMS authentication message that will be sent to users with the code they must sign in. The message must contain the \\u2018{####}\\u2019 placeholder, which is replaced with the code. If the message isn't included, and default message will be used.\"\n        }\n      ]\n    },\n    \"SmsConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsConfigurationType\"\n        },\n        {\n          \"description\": \"The SMS configuration with the settings that your Amazon Cognito user pool must use to send an SMS message from your Amazon Web Services account through Amazon Simple Notification Service. To request Amazon SNS in the Amazon Web Services Region that you want, the Amazon Cognito user\
  \ pool uses an Identity and Access Management (IAM) role that you provide for your Amazon Web Services account.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The SMS text message multi-factor authentication (MFA) configuration type.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-sms-mfa-config-type-schema.json\",\n  \"title\": \"SmsMfaConfigType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-sms-mfa-config-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: SmsMfaConfigType
---
