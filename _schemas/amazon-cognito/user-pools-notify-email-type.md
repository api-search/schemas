---
description: The notify email type.
layout: schema
name: NotifyEmailType
properties_list:
- description: ''
  name: Subject
  type: object
- description: ''
  name: HtmlBody
  type: object
- description: ''
  name: TextBody
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-notify-email-type-schema.json
slug: user-pools-notify-email-type
source_filename: user-pools-notify-email-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-notify-email-type-schema.json\",\n  \"title\": \"NotifyEmailType\",\n  \"description\": \"The notify email type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Subject\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailNotificationSubjectType\"\n        },\n        {\n          \"description\": \"The email subject.\"\n        }\n      ]\n    },\n    \"HtmlBody\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailNotificationBodyType\"\n        },\n        {\n          \"description\": \"The email HTML body.\"\n        }\n      ]\n    },\n    \"TextBody\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmailNotificationBodyType\"\n        },\n        {\n          \"description\": \"The email\
  \ text body.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Subject\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-notify-email-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: NotifyEmailType
---
