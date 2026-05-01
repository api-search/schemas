---
description: A YouTube video resource as returned by the YouTube Data API v3.
layout: schema
name: YouTube Video
properties_list:
- description: ''
  name: kind
  type: string
- description: The ETag of the resource.
  name: etag
  type: string
- description: The ID that YouTube uses to uniquely identify the video.
  name: id
  type: string
- description: Basic details about the video, such as its title, description, and category.
  name: snippet
  type: object
- description: Information about the video content.
  name: contentDetails
  type: object
- description: Statistics about the video.
  name: statistics
  type: object
- description: The status of the video.
  name: status
  type: object
provider_name: YouTube Data
provider_slug: google-youtube
schema_file: json-schema/youtube.json
slug: youtube
source_filename: youtube.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-youtube/refs/heads/main/json-schema/youtube.json\",\n  \"title\": \"YouTube Video\",\n  \"description\": \"A YouTube video resource as returned by the YouTube Data API v3.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"const\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The ETag of the resource.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID that YouTube uses to uniquely identify the video.\"\n    },\n    \"snippet\": {\n      \"type\": \"object\",\n      \"description\": \"Basic details about the video, such as its title, description, and category.\",\n      \"properties\": {\n        \"publishedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\"\
  : \"The date and time the video was published.\"\n        },\n        \"channelId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the channel the video belongs to.\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The video's title.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The video's description.\"\n        },\n        \"thumbnails\": {\n          \"type\": \"object\",\n          \"description\": \"A map of thumbnail images associated with the video.\",\n          \"properties\": {\n            \"default\": {\n              \"$ref\": \"#/$defs/Thumbnail\"\n            },\n            \"medium\": {\n              \"$ref\": \"#/$defs/Thumbnail\"\n            },\n            \"high\": {\n              \"$ref\": \"#/$defs/Thumbnail\"\n            }\n          }\n        },\n        \"channelTitle\": {\n          \"type\": \"string\",\n          \"\
  description\": \"The channel title of the channel the video belongs to.\"\n        },\n        \"tags\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"A list of keyword tags associated with the video.\"\n        },\n        \"categoryId\": {\n          \"type\": \"string\",\n          \"description\": \"The YouTube video category associated with the video.\"\n        }\n      },\n      \"required\": [\"title\"]\n    },\n    \"contentDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the video content.\",\n      \"properties\": {\n        \"duration\": {\n          \"type\": \"string\",\n          \"description\": \"The length of the video in ISO 8601 duration format.\"\n        },\n        \"dimension\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates whether the video is 2D or 3D.\"\n        },\n        \"definition\": {\n          \"\
  type\": \"string\",\n          \"enum\": [\"hd\", \"sd\"],\n          \"description\": \"Indicates whether the video is HD or SD.\"\n        },\n        \"caption\": {\n          \"type\": \"string\",\n          \"enum\": [\"true\", \"false\"],\n          \"description\": \"Indicates whether captions are available.\"\n        }\n      }\n    },\n    \"statistics\": {\n      \"type\": \"object\",\n      \"description\": \"Statistics about the video.\",\n      \"properties\": {\n        \"viewCount\": {\n          \"type\": \"string\",\n          \"description\": \"The number of times the video has been viewed.\"\n        },\n        \"likeCount\": {\n          \"type\": \"string\",\n          \"description\": \"The number of users who liked the video.\"\n        },\n        \"dislikeCount\": {\n          \"type\": \"string\",\n          \"description\": \"The number of users who disliked the video.\"\n        },\n        \"commentCount\": {\n          \"type\": \"string\",\n          \"\
  description\": \"The number of comments for the video.\"\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"description\": \"The status of the video.\",\n      \"properties\": {\n        \"uploadStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\"deleted\", \"failed\", \"processed\", \"rejected\", \"uploaded\"]\n        },\n        \"privacyStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\"private\", \"public\", \"unlisted\"]\n        },\n        \"embeddable\": {\n          \"type\": \"boolean\"\n        }\n      }\n    }\n  },\n  \"required\": [\"kind\", \"id\"],\n  \"$defs\": {\n    \"Thumbnail\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"width\": {\n          \"type\": \"integer\"\n        },\n        \"height\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-youtube/refs/heads/main/json-schema/youtube.json
tags:
- Channels
- Google
- Media
- Playlists
- Search
- Streaming
- Video
- YouTube
title: YouTube Video
---
