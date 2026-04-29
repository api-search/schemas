---
description: TopicDestinationRoute schema from Ampersand API
layout: schema
name: TopicDestinationRoute
properties_list:
- description: The topic destination route ID.
  name: id
  type: string
- description: The ID of the topic.
  name: topicId
  type: string
- description: The ID of the destination.
  name: destinationId
  type: string
- description: The Ampersand project ID.
  name: projectId
  type: string
- description: The time when the topic destination route was created.
  name: createTime
  type: string
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-topic-destination-route-schema.json
slug: ampersand-api-topic-destination-route
source_filename: ampersand-api-topic-destination-route-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-topic-destination-route-schema.json\",\n  \"title\": \"TopicDestinationRoute\",\n  \"description\": \"TopicDestinationRoute schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The topic destination route ID.\"\n    },\n    \"topicId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the topic.\"\n    },\n    \"destinationId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the destination.\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The Ampersand project ID.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the topic destination route was\
  \ created.\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"topicId\",\n    \"destinationId\",\n    \"projectId\",\n    \"createTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-topic-destination-route-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: TopicDestinationRoute
---
