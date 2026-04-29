---
description: The template for verification messages.
layout: schema
name: VerificationMessageTemplateType
properties_list:
- description: ''
  name: SmsMessage
  type: object
- description: ''
  name: EmailMessage
  type: object
- description: ''
  name: EmailSubject
  type: object
- description: ''
  name: EmailMessageByLink
  type: object
- description: ''
  name: EmailSubjectByLink
  type: object
- description: ''
  name: DefaultEmailOption
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-verification-message-template-type-schema.json
slug: cognito-idp-verification-message-template-type
source_filename: cognito-idp-verification-message-template-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SmsMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsVerificationMessageType\"\n        },\n        {\n          \"description\": \"The template for SMS messages that Amazon Cognito sends to your users.\"\n        }\n      ]\n    },\n    \"EmailMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailVerificationMessageType\"\n        },\n        {\n          \"description\": \"The template for email messages that Amazon Cognito sends to your users. You can set an <code>EmailMessage</code> template only if the value of <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_EmailConfigurationType.html#CognitoUserPools-Type-EmailConfigurationType-EmailSendingAccount\\\"> EmailSendingAccount</a> is <code>DEVELOPER</code>. When your <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_EmailConfigurationType.html#CognitoUserPools-Type-EmailConfigurationType-EmailSendingAccount\\\
  \">EmailSendingAccount</a> is <code>DEVELOPER</code>, your user pool sends email messages with your own Amazon SES configuration.\"\n        }\n      ]\n    },\n    \"EmailSubject\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailVerificationSubjectType\"\n        },\n        {\n          \"description\": \"The subject line for the email message template. You can set an <code>EmailSubject</code> template only if the value of <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_EmailConfigurationType.html#CognitoUserPools-Type-EmailConfigurationType-EmailSendingAccount\\\"> EmailSendingAccount</a> is <code>DEVELOPER</code>. When your <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_EmailConfigurationType.html#CognitoUserPools-Type-EmailConfigurationType-EmailSendingAccount\\\">EmailSendingAccount</a> is <code>DEVELOPER</code>, your user pool sends email messages with your\
  \ own Amazon SES configuration.\"\n        }\n      ]\n    },\n    \"EmailMessageByLink\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailVerificationMessageByLinkType\"\n        },\n        {\n          \"description\": \"The email message template for sending a confirmation link to the user. You can set an <code>EmailMessageByLink</code> template only if the value of <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_EmailConfigurationType.html#CognitoUserPools-Type-EmailConfigurationType-EmailSendingAccount\\\"> EmailSendingAccount</a> is <code>DEVELOPER</code>. When your <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_EmailConfigurationType.html#CognitoUserPools-Type-EmailConfigurationType-EmailSendingAccount\\\">EmailSendingAccount</a> is <code>DEVELOPER</code>, your user pool sends email messages with your own Amazon SES configuration.\"\n        }\n      ]\n  \
  \  },\n    \"EmailSubjectByLink\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailVerificationSubjectByLinkType\"\n        },\n        {\n          \"description\": \"The subject line for the email message template for sending a confirmation link to the user. You can set an <code>EmailSubjectByLink</code> template only if the value of <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_EmailConfigurationType.html#CognitoUserPools-Type-EmailConfigurationType-EmailSendingAccount\\\"> EmailSendingAccount</a> is <code>DEVELOPER</code>. When your <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_EmailConfigurationType.html#CognitoUserPools-Type-EmailConfigurationType-EmailSendingAccount\\\">EmailSendingAccount</a> is <code>DEVELOPER</code>, your user pool sends email messages with your own Amazon SES configuration.\"\n        }\n      ]\n    },\n    \"DefaultEmailOption\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultEmailOptionType\"\n        },\n        {\n          \"description\": \"The default email option.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The template for verification messages.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-verification-message-template-type-schema.json\",\n  \"title\": \"VerificationMessageTemplateType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-verification-message-template-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: VerificationMessageTemplateType
---
