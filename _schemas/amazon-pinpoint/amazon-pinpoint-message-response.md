---
description: Provides information about the results of a request to send a message to an endpoint address.
layout: schema
name: MessageResponse
properties_list:
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: EndpointResult
  type: object
- description: ''
  name: RequestId
  type: object
- description: ''
  name: Result
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-message-response-schema.json
slug: amazon-pinpoint-message-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-message-response-schema.json\",\n  \"title\": \"MessageResponse\",\n  \"description\": \"Provides information about the results of a request to send a message to an endpoint address.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application that was used to send the message.\"\n        }\n      ]\n    },\n    \"EndpointResult\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfEndpointMessageResult\"\n        },\n        {\n          \"description\": \"A map that contains a multipart response for each address that the message was sent to. In the map, the endpoint\
  \ ID is the key and the result is the value.\"\n        }\n      ]\n    },\n    \"RequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The identifier for the original request that the message was delivered for.\"\n        }\n      ]\n    },\n    \"Result\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfMessageResult\"\n        },\n        {\n          \"description\": \"A map that contains a multipart response for each address (email address, phone number, or push notification token) that the message was sent to. In the map, the address is the key and the result is the value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-message-response-schema.json
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
title: MessageResponse
---
