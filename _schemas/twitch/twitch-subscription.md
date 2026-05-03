---
description: Represents a channel subscription on Twitch, including the subscriber, broadcaster, tier level, and gift information.
layout: schema
name: Twitch Subscription
properties_list:
- description: ID of the broadcaster being subscribed to
  name: broadcaster_id
  type: string
- description: Login name of the broadcaster
  name: broadcaster_login
  type: string
- description: Display name of the broadcaster
  name: broadcaster_name
  type: string
- description: ID of the user who gifted the subscription (empty if not a gift)
  name: gifter_id
  type: string
- description: Login name of the gifter
  name: gifter_login
  type: string
- description: Display name of the gifter
  name: gifter_name
  type: string
- description: Whether the subscription is a gift
  name: is_gift
  type: boolean
- description: Name of the subscription plan
  name: plan_name
  type: string
- description: Subscription tier (1000=Tier 1, 2000=Tier 2, 3000=Tier 3)
  name: tier
  type: string
- description: ID of the subscribed user
  name: user_id
  type: string
- description: Display name of the subscribed user
  name: user_name
  type: string
- description: Login name of the subscribed user
  name: user_login
  type: string
provider_name: Twitch
provider_slug: twitch
schema_file: json-schema/twitch-subscription-schema.json
slug: twitch-subscription
source_filename: twitch-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://dev.twitch.tv/schemas/twitch/subscription.json\",\n  \"title\": \"Twitch Subscription\",\n  \"description\": \"Represents a channel subscription on Twitch, including the subscriber, broadcaster, tier level, and gift information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"broadcaster_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the broadcaster being subscribed to\"\n    },\n    \"broadcaster_login\": {\n      \"type\": \"string\",\n      \"description\": \"Login name of the broadcaster\"\n    },\n    \"broadcaster_name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the broadcaster\"\n    },\n    \"gifter_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who gifted the subscription (empty if not a gift)\"\n    },\n    \"gifter_login\": {\n      \"type\": \"string\",\n      \"description\": \"Login\
  \ name of the gifter\"\n    },\n    \"gifter_name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the gifter\"\n    },\n    \"is_gift\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the subscription is a gift\"\n    },\n    \"plan_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the subscription plan\"\n    },\n    \"tier\": {\n      \"type\": \"string\",\n      \"enum\": [\"1000\", \"2000\", \"3000\"],\n      \"description\": \"Subscription tier (1000=Tier 1, 2000=Tier 2, 3000=Tier 3)\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the subscribed user\"\n    },\n    \"user_name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the subscribed user\"\n    },\n    \"user_login\": {\n      \"type\": \"string\",\n      \"description\": \"Login name of the subscribed user\"\n    }\n  },\n  \"required\": [\"broadcaster_id\", \"broadcaster_login\", \"broadcaster_name\"\
  , \"is_gift\", \"tier\", \"user_id\", \"user_name\", \"user_login\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitch/refs/heads/main/json-schema/twitch-subscription-schema.json
tags:
- Entertainment
- Gaming
- Live Video
- Streaming
- Video
title: Twitch Subscription
---
