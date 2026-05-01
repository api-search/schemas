---
description: Specifies information about an event that reports data to Amazon Pinpoint.
layout: schema
name: Event
properties_list:
- description: ''
  name: AppPackageName
  type: object
- description: ''
  name: AppTitle
  type: object
- description: ''
  name: AppVersionCode
  type: object
- description: ''
  name: Attributes
  type: object
- description: ''
  name: ClientSdkVersion
  type: object
- description: ''
  name: EventType
  type: object
- description: ''
  name: Metrics
  type: object
- description: ''
  name: SdkName
  type: object
- description: ''
  name: Session
  type: object
- description: ''
  name: Timestamp
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-event-schema.json
slug: amazon-pinpoint-event
source_filename: amazon-pinpoint-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-event-schema.json\",\n  \"title\": \"Event\",\n  \"description\": \"Specifies information about an event that reports data to Amazon Pinpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AppPackageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The package name of the app that's recording the event.\"\n        }\n      ]\n    },\n    \"AppTitle\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The title of the app that's recording the event.\"\n        }\n      ]\n    },\n    \"AppVersionCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n\
  \        },\n        {\n          \"description\": \"The version number of the app that's recording the event.\"\n        }\n      ]\n    },\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"One or more custom attributes that are associated with the event.\"\n        }\n      ]\n    },\n    \"ClientSdkVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The version of the SDK that's running on the client device.\"\n        }\n      ]\n    },\n    \"EventType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the event.\"\n        }\n      ]\n    },\n    \"Metrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__double\"\n        },\n\
  \        {\n          \"description\": \"One or more custom metrics that are associated with the event.\"\n        }\n      ]\n    },\n    \"SdkName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the SDK that's being used to record the event.\"\n        }\n      ]\n    },\n    \"Session\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Session\"\n        },\n        {\n          \"description\": \"Information about the session in which the event occurred.\"\n        }\n      ]\n    },\n    \"Timestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and time, in ISO 8601 format, when the event occurred.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EventType\",\n    \"Timestamp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-event-schema.json
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
title: Event
---
