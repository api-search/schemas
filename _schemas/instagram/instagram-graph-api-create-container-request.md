---
description: CreateContainerRequest schema from Instagram Graph API
layout: schema
name: CreateContainerRequest
properties_list:
- description: Public URL of the image to publish.
  name: image_url
  type: string
- description: Public URL of the video to publish.
  name: video_url
  type: string
- description: Caption text for the media.
  name: caption
  type: string
- description: Type of media to publish.
  name: media_type
  type: string
- description: Set to true if this is an item in a carousel.
  name: is_carousel_item
  type: boolean
- description: Facebook Page ID of a location to tag.
  name: location_id
  type: string
- description: Users to tag in the media.
  name: user_tags
  type: array
- description: ''
  name: access_token
  type: string
provider_name: Instagram
provider_slug: instagram
schema_file: json-schema/instagram-graph-api-create-container-request-schema.json
slug: instagram-graph-api-create-container-request
source_filename: instagram-graph-api-create-container-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-create-container-request-schema.json\",\n  \"title\": \"CreateContainerRequest\",\n  \"description\": \"CreateContainerRequest schema from Instagram Graph API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"image_url\": {\n      \"type\": \"string\",\n      \"description\": \"Public URL of the image to publish.\",\n      \"example\": \"https://www.example.com/images/photo.jpg\"\n    },\n    \"video_url\": {\n      \"type\": \"string\",\n      \"description\": \"Public URL of the video to publish.\"\n    },\n    \"caption\": {\n      \"type\": \"string\",\n      \"description\": \"Caption text for the media.\",\n      \"example\": \"Check out our latest product! #newlaunch\"\n    },\n    \"media_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of media to publish.\"\
  ,\n      \"enum\": [\n        \"IMAGE\",\n        \"VIDEO\",\n        \"REELS\",\n        \"STORIES\",\n        \"CAROUSEL\"\n      ],\n      \"example\": \"IMAGE\"\n    },\n    \"is_carousel_item\": {\n      \"type\": \"boolean\",\n      \"description\": \"Set to true if this is an item in a carousel.\",\n      \"example\": false\n    },\n    \"location_id\": {\n      \"type\": \"string\",\n      \"description\": \"Facebook Page ID of a location to tag.\"\n    },\n    \"user_tags\": {\n      \"type\": \"array\",\n      \"description\": \"Users to tag in the media.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"username\": {\n            \"type\": \"string\"\n          },\n          \"x\": {\n            \"type\": \"number\"\n          },\n          \"y\": {\n            \"type\": \"number\"\n          }\n        }\n      }\n    },\n    \"access_token\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/json-schema/instagram-graph-api-create-container-request-schema.json
tags:
- Instagram
- Meta
- Photos
- Social Media
- Videos
- Content Publishing
title: CreateContainerRequest
---
