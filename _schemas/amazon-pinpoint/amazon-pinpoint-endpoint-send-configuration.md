---
description: Specifies the content, including message variables and attributes, to use in a message that's sent directly to an endpoint.
layout: schema
name: EndpointSendConfiguration
properties_list:
- description: ''
  name: BodyOverride
  type: object
- description: ''
  name: Context
  type: object
- description: ''
  name: RawContent
  type: object
- description: ''
  name: Substitutions
  type: object
- description: ''
  name: TitleOverride
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-endpoint-send-configuration-schema.json
slug: amazon-pinpoint-endpoint-send-configuration
source_filename: amazon-pinpoint-endpoint-send-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-send-configuration-schema.json\",\n  \"title\": \"EndpointSendConfiguration\",\n  \"description\": \"Specifies the content, including message variables and attributes, to use in a message that's sent directly to an endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BodyOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The body of the message. If specified, this value overrides the default message body.\"\n        }\n      ]\n    },\n    \"Context\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"<p>A map of custom attributes to attach to the message for the address.\
  \ Attribute names are case sensitive.</p> <p>For a push notification, this payload is added to the data.pinpoint object. For an email or text message, this payload is added to email/SMS delivery receipt event attributes.</p>\"\n        }\n      ]\n    },\n    \"RawContent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The raw, JSON-formatted string to use as the payload for the message. If specified, this value overrides all other values for the message.\"\n        }\n      ]\n    },\n    \"Substitutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfListOf__string\"\n        },\n        {\n          \"description\": \"A map of the message variables to merge with the variables specified for the default message (DefaultMessage.Substitutions). The variables specified in this map take precedence over all other variables.\"\n        }\n      ]\n    },\n   \
  \ \"TitleOverride\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The title or subject line of the message. If specified, this value overrides the default message title or subject line.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-send-configuration-schema.json
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
title: EndpointSendConfiguration
---
