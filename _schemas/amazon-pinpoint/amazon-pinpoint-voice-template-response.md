---
description: Provides information about the content and settings for a message template that can be used in messages that are sent through the voice channel.
layout: schema
name: VoiceTemplateResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Body
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: DefaultSubstitutions
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: TemplateDescription
  type: object
- description: ''
  name: TemplateName
  type: object
- description: ''
  name: TemplateType
  type: object
- description: ''
  name: Version
  type: object
- description: ''
  name: VoiceId
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-voice-template-response-schema.json
slug: amazon-pinpoint-voice-template-response
source_filename: amazon-pinpoint-voice-template-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-voice-template-response-schema.json\",\n  \"title\": \"VoiceTemplateResponse\",\n  \"description\": \"Provides information about the content and settings for a message template that can be used in messages that are sent through the voice channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the message template.\"\n        }\n      ]\n    },\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The text of the script that's used in messages that are based on the message template, in plain text format.\"\
  \n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in ISO 8601 format, when the message template was created.\"\n        }\n      ]\n    },\n    \"DefaultSubstitutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The JSON object that specifies the default values that are used for message variables in the message template. This object is a set of key-value pairs. Each key defines a message variable in the template. The corresponding value defines the default value for that variable.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The code for the language that's used when synthesizing the text of\
  \ the script in messages that are based on the message template. For a list of supported languages and the code for each one, see the <a href=\\\"https://docs.aws.amazon.com/polly/latest/dg/what-is.html\\\">Amazon Polly Developer Guide</a>.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in ISO 8601 format, when the message template was last modified.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"A string-to-string map of key-value pairs that identifies the tags that are associated with the message template. Each tag consists of a required tag key and an associated tag value.\"\n        }\n      ]\n    },\n    \"TemplateDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom description of the message template.\"\n        }\n      ]\n    },\n    \"TemplateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the message template.\"\n        }\n      ]\n    },\n    \"TemplateType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateType\"\n        },\n        {\n          \"description\": \"The type of channel that the message template is designed for. For a voice template, this value is VOICE.\"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier, as an integer, for the active version of the message template, or the version of the template that you specified by using\
  \ the version parameter in your request.\"\n        }\n      ]\n    },\n    \"VoiceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the voice that's used when delivering messages that are based on the message template. For a list of supported voices, see the <a href=\\\"https://docs.aws.amazon.com/polly/latest/dg/what-is.html\\\">Amazon Polly Developer Guide</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LastModifiedDate\",\n    \"CreationDate\",\n    \"TemplateName\",\n    \"TemplateType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-voice-template-response-schema.json
tags:
- AWS
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
title: VoiceTemplateResponse
---
