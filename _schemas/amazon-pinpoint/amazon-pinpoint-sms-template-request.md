---
description: Specifies the content and settings for a message template that can be used in text messages that are sent through the SMS channel.
layout: schema
name: SMSTemplateRequest
properties_list:
- description: ''
  name: Body
  type: object
- description: ''
  name: DefaultSubstitutions
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
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-sms-template-request-schema.json
slug: amazon-pinpoint-sms-template-request
source_filename: amazon-pinpoint-sms-template-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-sms-template-request-schema.json\",\n  \"title\": \"SMSTemplateRequest\",\n  \"description\": \"Specifies the content and settings for a message template that can be used in text messages that are sent through the SMS channel.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The message body to use in text messages that are based on the message template.\"\n        }\n      ]\n    },\n    \"DefaultSubstitutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A JSON object that specifies the default values to use for message variables in the\
  \ message template. This object is a set of key-value pairs. Each key defines a message variable in the template. The corresponding value defines the default value for that variable. When you create a message that's based on the template, you can override these defaults with message-specific and address-specific variables and values.\"\n        }\n      ]\n    },\n    \"RecommenderId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the recommender model to use for the message template. Amazon Pinpoint uses this value to determine how to retrieve and process data from a recommender model when it sends messages that use the template, if the template contains message variables for recommendation data.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n        \
  \  \"description\": \"A string-to-string map of key-value pairs that defines the tags to associate with the message template. Each tag consists of a required tag key and an associated tag value.\"\n        }\n      ]\n    },\n    \"TemplateDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A custom description of the message template.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-sms-template-request-schema.json
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
title: SMSTemplateRequest
---
