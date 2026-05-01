---
description: Specifies the message template to use for the message, for each type of channel.
layout: schema
name: TemplateConfiguration
properties_list:
- description: ''
  name: EmailTemplate
  type: object
- description: ''
  name: PushTemplate
  type: object
- description: ''
  name: SMSTemplate
  type: object
- description: ''
  name: VoiceTemplate
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-template-configuration-schema.json
slug: amazon-pinpoint-template-configuration
source_filename: amazon-pinpoint-template-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-template-configuration-schema.json\",\n  \"title\": \"TemplateConfiguration\",\n  \"description\": \"Specifies the message template to use for the message, for each type of channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EmailTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Template\"\n        },\n        {\n          \"description\": \"The email template to use for the message.\"\n        }\n      ]\n    },\n    \"PushTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Template\"\n        },\n        {\n          \"description\": \"The push notification template to use for the message.\"\n        }\n      ]\n    },\n    \"SMSTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/Template\"\n        },\n        {\n          \"description\": \"The SMS template to use for the message.\"\n        }\n      ]\n    },\n    \"VoiceTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Template\"\n        },\n        {\n          \"description\": \"The voice template to use for the message. This object isn't supported for campaigns.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-template-configuration-schema.json
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
title: TemplateConfiguration
---
