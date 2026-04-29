---
description: Specifies the configuration and other settings for a message to send to all the endpoints that are associated with a list of users.
layout: schema
name: SendUsersMessageRequest
properties_list:
- description: ''
  name: Context
  type: object
- description: ''
  name: MessageConfiguration
  type: object
- description: ''
  name: TemplateConfiguration
  type: object
- description: ''
  name: TraceId
  type: object
- description: ''
  name: Users
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-send-users-message-request-schema.json
slug: amazon-pinpoint-send-users-message-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-send-users-message-request-schema.json\",\n  \"title\": \"SendUsersMessageRequest\",\n  \"description\": \"Specifies the configuration and other settings for a message to send to all the endpoints that are associated with a list of users.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Context\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"A map of custom attribute-value pairs. For a push notification, Amazon Pinpoint adds these attributes to the data.pinpoint object in the body of the notification payload. Amazon Pinpoint also provides these attributes in the events that it generates for users-messages deliveries.\"\n        }\n      ]\n    },\n    \"MessageConfiguration\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectMessageConfiguration\"\n        },\n        {\n          \"description\": \"The settings and content for the default message and any default messages that you defined for specific channels.\"\n        }\n      ]\n    },\n    \"TemplateConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateConfiguration\"\n        },\n        {\n          \"description\": \"The message template to use for the message.\"\n        }\n      ]\n    },\n    \"TraceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for tracing the message. This identifier is visible to message recipients.\"\n        }\n      ]\n    },\n    \"Users\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfEndpointSendConfiguration\"\n        },\n        {\n \
  \         \"description\": \"A map that associates user IDs with <a href=\\\"https://docs.aws.amazon.com/pinpoint/latest/apireference/apps-application-id-messages.html#apps-application-id-messages-model-endpointsendconfiguration\\\">EndpointSendConfiguration</a> objects. You can use an <a href=\\\"https://docs.aws.amazon.com/pinpoint/latest/apireference/apps-application-id-messages.html#apps-application-id-messages-model-endpointsendconfiguration\\\">EndpointSendConfiguration</a> object to tailor the message for a user by specifying settings such as content overrides and message variables.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MessageConfiguration\",\n    \"Users\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-send-users-message-request-schema.json
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
title: SendUsersMessageRequest
---
