---
description: A subscription resource contains information about a YouTube user's subscription to a channel.
layout: schema
name: Subscription
properties_list:
- description: Identifies the API resource's type. Value is youtube#subscription.
  name: kind
  type: string
- description: The Etag of this resource.
  name: etag
  type: string
- description: The ID that YouTube uses to uniquely identify the subscription.
  name: id
  type: string
- description: The snippet object contains basic details about the subscription.
  name: snippet
  type: object
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-subscription-schema.json
slug: youtube-data-subscription
source_filename: youtube-data-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A subscription resource contains information about a YouTube user's subscription to a channel.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#subscription.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID that YouTube uses to uniquely identify the subscription.\",\n      \"example\": \"abc123def456\"\n    },\n    \"snippet\": {\n      \"type\": \"object\",\n      \"description\": \"The snippet object contains basic details about the subscription.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"publishedAt\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The date and time that the subscription was created.\",\n          \"format\": \"date-time\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The subscription title.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The subscription description.\"\n        },\n        \"resourceId\": {\n          \"type\": \"object\",\n          \"description\": \"The resourceId object contains information about the resource to which the subscriber subscribed.\",\n          \"properties\": {\n            \"kind\": {\n              \"type\": \"string\",\n              \"description\": \"The type of the API resource.\"\n            },\n            \"channelId\": {\n              \"type\": \"string\",\n              \"description\": \"The value that YouTube uses to uniquely identify the channel that the user subscribed to.\"\n            }\n          }\n        },\n        \"channelId\": {\n        \
  \  \"type\": \"string\",\n          \"description\": \"The ID of the channel that the subscription belongs to.\"\n        },\n        \"thumbnails\": {\n          \"type\": \"object\",\n          \"description\": \"A map of thumbnail images associated with the subscription.\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"kind\",\n    \"etag\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Subscription\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-subscription-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: Subscription
---
