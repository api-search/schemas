---
description: Provides information about an application.
layout: schema
name: ApplicationResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: CreationDate
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-application-response-schema.json
slug: amazon-pinpoint-application-response
source_filename: amazon-pinpoint-application-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-application-response-schema.json\",\n  \"title\": \"ApplicationResponse\",\n  \"description\": \"Provides information about an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the application.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the application. This identifier is displayed as the <b>Project ID</b> on the Amazon Pinpoint console.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n         \
  \ \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The display name of the application. This name is displayed as the <b>Project name</b> on the Amazon Pinpoint console.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"A string-to-string map of key-value pairs that identifies the tags that are associated with the application. Each tag consists of a required tag key and an associated tag value.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The date and time when the Application was created.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Id\",\n    \"Arn\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-application-response-schema.json
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
title: ApplicationResponse
---
