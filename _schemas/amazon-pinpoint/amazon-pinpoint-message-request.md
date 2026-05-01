---
description: Specifies the configuration and other settings for a message.
layout: schema
name: MessageRequest
properties_list:
- description: ''
  name: Addresses
  type: object
- description: ''
  name: Context
  type: object
- description: ''
  name: Endpoints
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
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-message-request-schema.json
slug: amazon-pinpoint-message-request
source_filename: amazon-pinpoint-message-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-message-request-schema.json\",\n  \"title\": \"MessageRequest\",\n  \"description\": \"Specifies the configuration and other settings for a message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Addresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfAddressConfiguration\"\n        },\n        {\n          \"description\": \"A map of key-value pairs, where each key is an address and each value is an <a href=\\\"https://docs.aws.amazon.com/pinpoint/latest/apireference/apps-application-id-messages.html#apps-application-id-messages-model-addressconfiguration\\\">AddressConfiguration</a> object. An address can be a push notification token, a phone number, or an email address. You can use an <a href=\\\"https://docs.aws.amazon.com/pinpoint/latest/apireference/apps-application-id-messages.html#apps-application-id-messages-model-addressconfiguration\\\
  \">AddressConfiguration</a> object to tailor the message for an address by specifying settings such as content overrides and message variables.\"\n        }\n      ]\n    },\n    \"Context\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"A map of custom attributes to attach to the message. For a push notification, this payload is added to the data.pinpoint object. For an email or text message, this payload is added to email/SMS delivery receipt event attributes.\"\n        }\n      ]\n    },\n    \"Endpoints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfEndpointSendConfiguration\"\n        },\n        {\n          \"description\": \"A map of key-value pairs, where each key is an endpoint ID and each value is an <a href=\\\"https://docs.aws.amazon.com/pinpoint/latest/apireference/apps-application-id-messages.html#apps-application-id-messages-model-endpointsendconfiguration\\\
  \">EndpointSendConfiguration</a> object. You can use an <a href=\\\"https://docs.aws.amazon.com/pinpoint/latest/apireference/apps-application-id-messages.html#apps-application-id-messages-model-endpointsendconfiguration\\\">EndpointSendConfiguration</a> object to tailor the message for an endpoint by specifying settings such as content overrides and message variables.\"\n        }\n      ]\n    },\n    \"MessageConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectMessageConfiguration\"\n        },\n        {\n          \"description\": \"The settings and content for the default message and any default messages that you defined for specific channels.\"\n        }\n      ]\n    },\n    \"TemplateConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateConfiguration\"\n        },\n        {\n          \"description\": \"The message template to use for the message.\"\n        }\n      ]\n    },\n  \
  \  \"TraceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for tracing the message. This identifier is visible to message recipients.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MessageConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-message-request-schema.json
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
title: MessageRequest
---
