---
description: The message template structure.
layout: schema
name: MessageTemplateType
properties_list:
- description: ''
  name: SMSMessage
  type: object
- description: ''
  name: EmailMessage
  type: object
- description: ''
  name: EmailSubject
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-message-template-type-schema.json
slug: user-pools-message-template-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-message-template-type-schema.json\",\n  \"title\": \"MessageTemplateType\",\n  \"description\": \"The message template structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SMSMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SmsVerificationMessageType\"\n        },\n        {\n          \"description\": \"The message template for SMS messages.\"\n        }\n      ]\n    },\n    \"EmailMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailVerificationMessageType\"\n        },\n        {\n          \"description\": \"The message template for email messages. EmailMessage is allowed only if <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_EmailConfigurationType.html#CognitoUserPools-Type-EmailConfigurationType-EmailSendingAccount\\\
  \">EmailSendingAccount</a> is DEVELOPER. \"\n        }\n      ]\n    },\n    \"EmailSubject\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailVerificationSubjectType\"\n        },\n        {\n          \"description\": \"The subject line for email messages. EmailSubject is allowed only if <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_EmailConfigurationType.html#CognitoUserPools-Type-EmailConfigurationType-EmailSendingAccount\\\">EmailSendingAccount</a> is DEVELOPER. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-message-template-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: MessageTemplateType
---
