---
description: An XActivity subscription.
layout: schema
name: ActivitySubscription
properties_list:
- description: ''
  name: created_at
  type: string
- description: ''
  name: event_type
  type: string
- description: An XAA subscription filter.
  name: filter
  type: object
- description: The unique identifier of this subscription.
  name: subscription_id
  type: string
- description: ''
  name: tag
  type: string
- description: ''
  name: updated_at
  type: string
- description: The unique identifier of this webhook config.
  name: webhook_id
  type: string
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-activity-subscription-schema.json
slug: x-api-activity-subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-activity-subscription-schema.json\",\n  \"title\": \"ActivitySubscription\",\n  \"description\": \"An XActivity subscription.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"event_type\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"filter\": {\n      \"type\": \"object\",\n      \"description\": \"An XAA subscription filter.\",\n      \"properties\": {\n        \"direction\": {\n          \"type\": \"string\",\n          \"description\": \"Optional direction filter for directional events.\",\n          \"enum\": [\n            \"inbound\",\n            \"outbound\"\n          ],\n          \"example\": \"inbound\"\n        },\n\
  \        \"keyword\": {\n          \"$ref\": \"#/components/schemas/Keyword\"\n        },\n        \"user_id\": {\n          \"$ref\": \"#/components/schemas/UserId\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"subscription_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of this subscription.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"1146654567674912769\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"example\": \"example_tag\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"webhook_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of this webhook config.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"1146654567674912769\"\n    }\n  },\n  \"required\": [\n    \"subscription_id\",\n    \"event_type\",\n    \"filter\",\n    \"created_at\"\
  ,\n    \"updated_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-activity-subscription-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: ActivitySubscription
---
