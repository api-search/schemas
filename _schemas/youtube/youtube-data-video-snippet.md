---
description: Basic details about a video, including its title, description, tags, and category.
layout: schema
name: VideoSnippet
properties_list:
- description: The date and time when the video was published.
  name: publishedAt
  type: string
- description: The ID of the YouTube channel that published the video.
  name: channelId
  type: string
- description: The video title.
  name: title
  type: string
- description: The video description.
  name: description
  type: string
- description: A map of thumbnail images associated with the video.
  name: thumbnails
  type: object
- description: The channel title of the YouTube channel that published the video.
  name: channelTitle
  type: string
- description: A list of keyword tags associated with the video.
  name: tags
  type: array
- description: The YouTube video category associated with the video.
  name: categoryId
  type: string
- description: Indicates if the video is an upcoming/active live broadcast.
  name: liveBroadcastContent
  type: string
- description: The language of the text in the video resource's snippet.title and snippet.description properties.
  name: defaultLanguage
  type: string
- description: The snippet.localized object contains either a localized title and description for the video or the title in the default language.
  name: localized
  type: object
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-video-snippet-schema.json
slug: youtube-data-video-snippet
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Basic details about a video, including its title, description, tags, and category.\",\n  \"properties\": {\n    \"publishedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the video was published.\",\n      \"example\": \"2026-01-15T10:30:00Z\",\n      \"format\": \"date-time\"\n    },\n    \"channelId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the YouTube channel that published the video.\",\n      \"example\": \"500123\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The video title.\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The video description.\",\n      \"example\": \"A sample description for this resource.\"\n    },\n    \"thumbnails\": {\n      \"type\": \"object\",\n      \"description\": \"A map of thumbnail images associated with the\
  \ video.\",\n      \"example\": \"example_value\"\n    },\n    \"channelTitle\": {\n      \"type\": \"string\",\n      \"description\": \"The channel title of the YouTube channel that published the video.\",\n      \"example\": \"example_value\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"A list of keyword tags associated with the video.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"categoryId\": {\n      \"type\": \"string\",\n      \"description\": \"The YouTube video category associated with the video.\",\n      \"example\": \"500123\"\n    },\n    \"liveBroadcastContent\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates if the video is an upcoming/active live broadcast.\",\n      \"example\": \"live\",\n      \"enum\": [\n        \"live\",\n        \"none\",\n        \"upcoming\"\n      ]\n    },\n    \"defaultLanguage\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The language of the text in the video resource's snippet.title and snippet.description properties.\",\n      \"example\": \"en\"\n    },\n    \"localized\": {\n      \"type\": \"object\",\n      \"description\": \"The snippet.localized object contains either a localized title and description for the video or the title in the default language.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The localized video title.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The localized video description.\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VideoSnippet\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-video-snippet-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: VideoSnippet
---
