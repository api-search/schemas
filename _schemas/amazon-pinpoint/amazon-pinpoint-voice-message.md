---
description: Specifies the settings for a one-time voice message that's sent directly to an endpoint through the voice channel.
layout: schema
name: VoiceMessage
properties_list:
- description: ''
  name: Body
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: OriginationNumber
  type: object
- description: ''
  name: Substitutions
  type: object
- description: ''
  name: VoiceId
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-voice-message-schema.json
slug: amazon-pinpoint-voice-message
source_filename: amazon-pinpoint-voice-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-voice-message-schema.json\",\n  \"title\": \"VoiceMessage\",\n  \"description\": \"Specifies the settings for a one-time voice message that's sent directly to an endpoint through the voice channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The text of the script to use for the voice message.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The code for the language to use when synthesizing the text of the message script. For a list of supported languages and the code for each one, see\
  \ the <a href=\\\"https://docs.aws.amazon.com/polly/latest/dg/what-is.html\\\">Amazon Polly Developer Guide</a>.\"\n        }\n      ]\n    },\n    \"OriginationNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The long code to send the voice message from. This value should be one of the dedicated long codes that's assigned to your AWS account. Although it isn't required, we recommend that you specify the long code in E.164 format, for example +12065550100, to ensure prompt and accurate delivery of the message.\"\n        }\n      ]\n    },\n    \"Substitutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfListOf__string\"\n        },\n        {\n          \"description\": \"The default message variables to use in the voice message. You can override the default variables with individual address variables.\"\n        }\n      ]\n    },\n    \"VoiceId\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the voice to use when delivering the message. For a list of supported voices, see the <a href=\\\"https://docs.aws.amazon.com/polly/latest/dg/what-is.html\\\">Amazon Polly Developer Guide</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-voice-message-schema.json
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
title: VoiceMessage
---
