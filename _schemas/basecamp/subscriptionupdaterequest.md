---
description: ''
layout: schema
name: SubscriptionUpdateRequest
properties_list:
- description: Person IDs to add as subscribers
  name: subscriptions
  type: array
- description: Person IDs to remove as subscribers
  name: unsubscriptions
  type: array
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/subscriptionupdaterequest-schema.json
slug: subscriptionupdaterequest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/subscriptionupdaterequest-schema.json\",\n  \"title\": \"SubscriptionUpdateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subscriptions\": {\n      \"type\": \"array\",\n      \"description\": \"Person IDs to add as subscribers\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"unsubscriptions\": {\n      \"type\": \"array\",\n      \"description\": \"Person IDs to remove as subscribers\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/subscriptionupdaterequest-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: SubscriptionUpdateRequest
---
