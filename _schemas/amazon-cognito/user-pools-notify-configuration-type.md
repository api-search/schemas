---
description: The notify configuration type.
layout: schema
name: NotifyConfigurationType
properties_list:
- description: ''
  name: From
  type: object
- description: ''
  name: ReplyTo
  type: object
- description: ''
  name: SourceArn
  type: object
- description: ''
  name: BlockEmail
  type: object
- description: ''
  name: NoActionEmail
  type: object
- description: ''
  name: MfaEmail
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-notify-configuration-type-schema.json
slug: user-pools-notify-configuration-type
source_filename: user-pools-notify-configuration-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-notify-configuration-type-schema.json\",\n  \"title\": \"NotifyConfigurationType\",\n  \"description\": \"The notify configuration type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"From\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The email address that is sending the email. The address must be either individually verified with Amazon Simple Email Service, or from a domain that has been verified with Amazon SES.\"\n        }\n      ]\n    },\n    \"ReplyTo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The destination to which the receiver of an email should reply to.\"\n        }\n \
  \     ]\n    },\n    \"SourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the identity that is associated with the sending authorization policy. This identity permits Amazon Cognito to send for the email address specified in the <code>From</code> parameter.\"\n        }\n      ]\n    },\n    \"BlockEmail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotifyEmailType\"\n        },\n        {\n          \"description\": \"Email template used when a detected risk event is blocked.\"\n        }\n      ]\n    },\n    \"NoActionEmail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotifyEmailType\"\n        },\n        {\n          \"description\": \"The email template used when a detected risk event is allowed.\"\n        }\n      ]\n    },\n    \"MfaEmail\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/NotifyEmailType\"\n        },\n        {\n          \"description\": \"The multi-factor authentication (MFA) email template used when MFA is challenged as part of a detected risk.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-notify-configuration-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: NotifyConfigurationType
---
