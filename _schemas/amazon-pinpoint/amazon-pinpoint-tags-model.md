---
description: Specifies the tags (keys and values) for an application, campaign, message template, or segment.
layout: schema
name: TagsModel
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-tags-model-schema.json
slug: amazon-pinpoint-tags-model
source_filename: amazon-pinpoint-tags-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-tags-model-schema.json\",\n  \"title\": \"TagsModel\",\n  \"description\": \"Specifies the tags (keys and values) for an application, campaign, message template, or segment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapOf__string\"\n        },\n        {\n          \"description\": \"<p>A string-to-string map of key-value pairs that defines the tags for an application, campaign, message template, or segment. Each of these resources can have a maximum of 50 tags.</p> <p>Each tag consists of a required tag key and an associated tag value. The maximum length of a tag key is 128 characters. The maximum length of a tag value is 256 characters.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-tags-model-schema.json
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
title: TagsModel
---
