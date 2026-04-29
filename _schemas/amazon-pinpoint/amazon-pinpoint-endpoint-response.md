---
description: Provides information about the channel type and other settings for an endpoint.
layout: schema
name: EndpointResponse
properties_list:
- description: ''
  name: Address
  type: object
- description: ''
  name: ApplicationId
  type: object
- description: ''
  name: Attributes
  type: object
- description: ''
  name: ChannelType
  type: object
- description: ''
  name: CohortId
  type: object
- description: ''
  name: CreationDate
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
schema_file: json-schema/amazon-pinpoint-endpoint-response-schema.json
slug: amazon-pinpoint-endpoint-response
source_filename: amazon-pinpoint-endpoint-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-response-schema.json\",\n  \"title\": \"EndpointResponse\",\n  \"description\": \"Provides information about the channel type and other settings for an endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Address\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The destination address for messages or push notifications that you send to the endpoint. The address varies by channel. For example, the address for a push-notification channel is typically the token provided by a push notification service, such as an Apple Push Notification service (APNs) device token or a Firebase Cloud Messaging (FCM) registration token. The address for the SMS channel is a phone number in E.164\
  \ format, such as +12065550100. The address for the email channel is an email address.\"\n        }\n      ]\n    },\n    \"ApplicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application that's associated with the endpoint.\"\n        }\n      ]\n    },\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOfListOf__string\"\n        },\n        {\n          \"description\": \"One or more custom attributes that describe the endpoint by associating a name with an array of values. For example, the value of a custom attribute named Interests might be: [\\\"Science\\\", \\\"Music\\\", \\\"Travel\\\"]. You can use these attributes as filter criteria when you create segments.\"\n        }\n      ]\n    },\n    \"ChannelType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelType\"\
  \n        },\n        {\n          \"description\": \"The channel that's used when sending messages or push notifications to the endpoint.\"\n        }\n      ]\n    },\n    \"CohortId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A number from 0-99 that represents the cohort that the endpoint is assigned to. Endpoints are grouped into cohorts randomly, and each cohort contains approximately 1 percent of the endpoints for an application. Amazon Pinpoint assigns cohorts to the holdout or treatment allocations for campaigns.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and time, in ISO 8601 format, when the endpoint was created.\"\n        }\n      ]\n    },\n    \"Demographic\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/EndpointDemographic\"\n        },\n        {\n          \"description\": \"The demographic information for the endpoint, such as the time zone and platform.\"\n        }\n      ]\n    },\n    \"EffectiveDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and time, in ISO 8601 format, when the endpoint was last updated.\"\n        }\n      ]\n    },\n    \"EndpointStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>Specifies whether messages or push notifications are sent to the endpoint. Possible values are: ACTIVE, messages are sent to the endpoint; and, INACTIVE, messages aren\\u2019t sent to the endpoint.</p> <p>Amazon Pinpoint automatically sets this value to ACTIVE when you create an endpoint or update an existing endpoint. Amazon Pinpoint automatically sets\
  \ this value to INACTIVE if you update another endpoint that has the same address specified by the Address property.</p>\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier that you assigned to the endpoint. The identifier should be a globally unique identifier (GUID) to ensure that it doesn't conflict with other endpoint identifiers that are associated with the application.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointLocation\"\n        },\n        {\n          \"description\": \"The geographic information for the endpoint.\"\n        }\n      ]\n    },\n    \"Metrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__double\"\n        },\n        {\n          \"description\": \"One or more custom metrics that\
  \ your app reports to Amazon Pinpoint for the endpoint.\"\n        }\n      ]\n    },\n    \"OptOut\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Specifies whether the user who's associated with the endpoint has opted out of receiving messages and push notifications from you. Possible values are: ALL, the user has opted out and doesn't want to receive any messages or push notifications; and, NONE, the user hasn't opted out and wants to receive all messages and push notifications.\"\n        }\n      ]\n    },\n    \"RequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the most recent request to update the endpoint.\"\n        }\n      ]\n    },\n    \"User\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointUser\"\n        },\n \
  \       {\n          \"description\": \"One or more custom user attributes that your app reports to Amazon Pinpoint for the user who's associated with the endpoint.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-endpoint-response-schema.json
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
title: EndpointResponse
---
