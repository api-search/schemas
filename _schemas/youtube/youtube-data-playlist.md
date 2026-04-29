---
description: A playlist resource represents a YouTube playlist.
layout: schema
name: Playlist
properties_list:
- description: Identifies the API resource's type. Value is youtube#playlist.
  name: kind
  type: string
- description: The Etag of this resource.
  name: etag
  type: string
- description: The ID that YouTube uses to uniquely identify the playlist.
  name: id
  type: string
- description: Basic details about the playlist such as its title, description, and thumbnails.
  name: snippet
  type: object
- description: The status object contains status information for the playlist.
  name: status
  type: object
- description: The contentDetails object contains information about the playlist content.
  name: contentDetails
  type: object
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-playlist-schema.json
slug: youtube-data-playlist
source_filename: youtube-data-playlist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A playlist resource represents a YouTube playlist.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#playlist.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID that YouTube uses to uniquely identify the playlist.\",\n      \"example\": \"abc123def456\"\n    },\n    \"snippet\": {\n      \"type\": \"object\",\n      \"description\": \"Basic details about the playlist such as its title, description, and thumbnails.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"publishedAt\": {\n          \"type\": \"string\",\n          \"description\": \"The date and time that the\
  \ playlist was created.\",\n          \"format\": \"date-time\"\n        },\n        \"channelId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the channel that published the playlist.\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The playlist title.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The playlist description.\"\n        },\n        \"thumbnails\": {\n          \"type\": \"object\",\n          \"description\": \"A map of thumbnail images associated with the playlist.\"\n        },\n        \"channelTitle\": {\n          \"type\": \"string\",\n          \"description\": \"The channel title of the channel that the video belongs to.\"\n        },\n        \"tags\": {\n          \"type\": \"array\",\n          \"description\": \"Keyword tags associated with the playlist.\",\n          \"items\": {\n            \"type\": \"string\"\n     \
  \     }\n        },\n        \"defaultLanguage\": {\n          \"type\": \"string\",\n          \"description\": \"The language of the text in the playlist resource's snippet.title and snippet.description properties.\"\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"description\": \"The status object contains status information for the playlist.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"privacyStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The playlist's privacy status.\",\n          \"enum\": [\n            \"private\",\n            \"public\",\n            \"unlisted\"\n          ]\n        }\n      }\n    },\n    \"contentDetails\": {\n      \"type\": \"object\",\n      \"description\": \"The contentDetails object contains information about the playlist content.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"itemCount\": {\n          \"type\": \"integer\"\
  ,\n          \"description\": \"The number of videos in the playlist.\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"kind\",\n    \"etag\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Playlist\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-playlist-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: Playlist
---
