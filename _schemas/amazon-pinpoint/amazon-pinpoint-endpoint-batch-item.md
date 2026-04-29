---
description: Specifies an endpoint to create or update and the settings and attributes to set or change for the endpoint.
layout: schema
name: EndpointBatchItem
properties_list:
- description: ''
  name: Address
  type: object
- description: ''
  name: Attributes
  type: object
- description: ''
  name: ChannelType
  type: object
- description: ''
  name: Demographic
  type: object
- description: ''
  name: EffectiveDate
  type: object
- description: ''
  name: EndpointStatus
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: Location
  type: object
- description: ''
  name: Metrics
  type: object
- description: ''
  name: OptOut
  type: object
- description: ''
  name: RequestId
  type: object
- description: ''
  name: User
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-endpoint-batch-item-schema.json
slug: amazon-pinpoint-endpoint-batch-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-batch-item-schema.json\",\n  \"title\": \"EndpointBatchItem\",\n  \"description\": \"Specifies an endpoint to create or update and the settings and attributes to set or change for the endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Address\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The destination address for messages or push notifications that you send to the endpoint. The address varies by channel. For a push-notification channel, use the token provided by the push notification service, such as an Apple Push Notification service (APNs) device token or a Firebase Cloud Messaging (FCM) registration token. For the SMS channel, use a phone number in E.164 format,\
  \ such as +12065550100. For the email channel, use an email address.\"\n        }\n      ]\n    },\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfListOf__string\"\n        },\n        {\n          \"description\": \"<p>One or more custom attributes that describe the endpoint by associating a name with an array of values. For example, the value of a custom attribute named Interests might be: [\\\"Science\\\", \\\"Music\\\", \\\"Travel\\\"]. You can use these attributes as filter criteria when you create segments. Attribute names are case sensitive.</p> <p>An attribute name can contain up to 50 characters. An attribute value can contain up to 100 characters. When you define the name of a custom attribute, avoid using the following characters: number sign (#), colon (:), question mark (?), backslash (\\\\), and slash (/). The Amazon Pinpoint console can't display attribute names that contain these characters. This restriction doesn't\
  \ apply to attribute values.</p>\"\n        }\n      ]\n    },\n    \"ChannelType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelType\"\n        },\n        {\n          \"description\": \"The channel to use when sending messages or push notifications to the endpoint.\"\n        }\n      ]\n    },\n    \"Demographic\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointDemographic\"\n        },\n        {\n          \"description\": \"The demographic information for the endpoint, such as the time zone and platform.\"\n        }\n      ]\n    },\n    \"EffectiveDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and time, in ISO 8601 format, when the endpoint was created or updated.\"\n        }\n      ]\n    },\n    \"EndpointStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"description\": \"<p>Specifies whether to send messages or push notifications to the endpoint. Valid values are: ACTIVE, messages are sent to the endpoint; and, INACTIVE, messages aren\\u2019t sent to the endpoint.</p> <p>Amazon Pinpoint automatically sets this value to ACTIVE when you create an endpoint or update an existing endpoint. Amazon Pinpoint automatically sets this value to INACTIVE if you update another endpoint that has the same address specified by the Address property.</p>\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the endpoint in the context of the batch.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointLocation\"\n        },\n        {\n          \"description\": \"The geographic information\
  \ for the endpoint.\"\n        }\n      ]\n    },\n    \"Metrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__double\"\n        },\n        {\n          \"description\": \"One or more custom metrics that your app reports to Amazon Pinpoint for the endpoint.\"\n        }\n      ]\n    },\n    \"OptOut\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Specifies whether the user who's associated with the endpoint has opted out of receiving messages and push notifications from you. Possible values are: ALL, the user has opted out and doesn't want to receive any messages or push notifications; and, NONE, the user hasn't opted out and wants to receive all messages and push notifications.\"\n        }\n      ]\n    },\n    \"RequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"\
  description\": \"The unique identifier for the request to create or update the endpoint.\"\n        }\n      ]\n    },\n    \"User\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointUser\"\n        },\n        {\n          \"description\": \"One or more custom attributes that describe the user who's associated with the endpoint.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-batch-item-schema.json
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
title: EndpointBatchItem
---
