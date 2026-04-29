---
description: Specifies the display name of an application and the tags to associate with the application.
layout: schema
name: CreateApplicationRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-create-application-request-schema.json
slug: amazon-pinpoint-create-application-request
source_filename: amazon-pinpoint-create-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-create-application-request-schema.json\",\n  \"title\": \"CreateApplicationRequest\",\n  \"description\": \"Specifies the display name of an application and the tags to associate with the application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The display name of the application. This name is displayed as the <b>Project name</b> on the Amazon Pinpoint console.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"A string-to-string map of key-value pairs that defines the tags to associate with\
  \ the application. Each tag consists of a required tag key and an associated tag value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-create-application-request-schema.json
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
title: CreateApplicationRequest
---
