---
description: ''
layout: schema
name: Subscription
properties_list:
- description: Whether the authenticated user is subscribed
  name: subscribed
  type: boolean
- description: Total number of subscribers
  name: count
  type: integer
- description: API URL for this subscription resource
  name: url
  type: string
- description: List of subscribed people
  name: subscribers
  type: array
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/subscription-schema.json
slug: subscription
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/subscription-schema.json\",\n  \"title\": \"Subscription\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subscribed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the authenticated user is subscribed\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of subscribers\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL for this subscription resource\"\n    },\n    \"subscribers\": {\n      \"type\": \"array\",\n      \"description\": \"List of subscribed people\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PersonRef\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/subscription-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Subscription
---
