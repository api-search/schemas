---
description: Specifies the status and settings of the email channel for an application.
layout: schema
name: EmailChannelRequest
properties_list:
- description: ''
  name: ConfigurationSet
  type: object
- description: ''
  name: Enabled
  type: object
- description: ''
  name: FromAddress
  type: object
- description: ''
  name: Identity
  type: object
- description: ''
  name: RoleArn
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-email-channel-request-schema.json
slug: amazon-pinpoint-email-channel-request
source_filename: amazon-pinpoint-email-channel-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-email-channel-request-schema.json\",\n  \"title\": \"EmailChannelRequest\",\n  \"description\": \"Specifies the status and settings of the email channel for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/ses/latest/APIReference/API_ConfigurationSet.html\\\">Amazon SES configuration set</a> that you want to apply to messages that you send through the channel.\"\n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether\
  \ to enable the email channel for the application.\"\n        }\n      ]\n    },\n    \"FromAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \" <p>The verified email address that you want to send email from when you send email through the channel.</p>\"\n        }\n      ]\n    },\n    \"Identity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \" <p>The Amazon Resource Name (ARN) of the identity, verified with Amazon Simple Email Service (Amazon SES), that you want to use when you send email through the channel.</p>\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \" <p>The ARN of the AWS Identity and Access Management (IAM) role that you want Amazon Pinpoint\
  \ to use when it submits email-related event data for the channel.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FromAddress\",\n    \"Identity\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-email-channel-request-schema.json
tags:
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: EmailChannelRequest
---
