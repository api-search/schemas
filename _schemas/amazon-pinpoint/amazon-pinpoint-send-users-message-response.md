---
description: Provides information about which users and endpoints a message was sent to.
layout: schema
name: SendUsersMessageResponse
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: RequestId
  type: object
- description: ''
  name: Result
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-send-users-message-response-schema.json
slug: amazon-pinpoint-send-users-message-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-send-users-message-response-schema.json\",\n  \"title\": \"SendUsersMessageResponse\",\n  \"description\": \"Provides information about which users and endpoints a message was sent to.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application that was used to send the message.\"\n        }\n      ]\n    },\n    \"RequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier that was assigned to the message request.\"\n        }\n      ]\n    },\n    \"Result\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/MapOfMapOfEndpointMessageResult\"\n        },\n        {\n          \"description\": \"An object that indicates which endpoints the message was sent to, for each user. The object lists user IDs and, for each user ID, provides the endpoint IDs that the message was sent to. For each endpoint ID, it provides an EndpointMessageResult object.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-send-users-message-response-schema.json
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
title: SendUsersMessageResponse
---
