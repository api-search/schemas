---
description: Provides information about the content and settings for a message template that can be used in text messages that are sent through the SMS channel.
layout: schema
name: SMSTemplateResponse
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
  name: LastModifiedDate
  type: object
- description: ''
  name: RecommenderId
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
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-sms-template-response-schema.json
slug: amazon-pinpoint-sms-template-response
source_filename: amazon-pinpoint-sms-template-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-sms-template-response-schema.json\",\n  \"title\": \"SMSTemplateResponse\",\n  \"description\": \"Provides information about the content and settings for a message template that can be used in text messages that are sent through the SMS channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the message template.\"\n        }\n      ]\n    },\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The message body that's used in text messages that are based on the message template.\"\n        }\n    \
  \  ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in ISO 8601 format, when the message template was created.\"\n        }\n      ]\n    },\n    \"DefaultSubstitutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The JSON object that specifies the default values that are used for message variables in the message template. This object is a set of key-value pairs. Each key defines a message variable in the template. The corresponding value defines the default value for that variable.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date, in ISO 8601 format, when the message template was last modified.\"\n \
  \       }\n      ]\n    },\n    \"RecommenderId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the recommender model that's used by the message template.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"A string-to-string map of key-value pairs that identifies the tags that are associated with the message template. Each tag consists of a required tag key and an associated tag value.\"\n        }\n      ]\n    },\n    \"TemplateDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The custom description of the message template.\"\n        }\n      ]\n    },\n    \"TemplateName\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the message template.\"\n        }\n      ]\n    },\n    \"TemplateType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateType\"\n        },\n        {\n          \"description\": \"The type of channel that the message template is designed for. For an SMS template, this value is SMS.\"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier, as an integer, for the active version of the message template, or the version of the template that you specified by using the version parameter in your request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LastModifiedDate\",\n    \"CreationDate\",\n    \"TemplateName\",\n    \"TemplateType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-sms-template-response-schema.json
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
title: SMSTemplateResponse
---
