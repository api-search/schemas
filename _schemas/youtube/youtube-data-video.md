---
description: A video resource represents a YouTube video.
layout: schema
name: Video
properties_list:
- description: Identifies the API resource's type. Value is youtube#video.
  name: kind
  type: string
- description: The Etag of this resource.
  name: etag
  type: string
- description: The ID that YouTube uses to uniquely identify the video.
  name: id
  type: string
- description: Basic details about a video, including its title, description, tags, and category.
  name: snippet
  type: object
- description: Information about the video content, including the length of the video and an indication of whether captions are available.
  name: contentDetails
  type: object
- description: The status of an uploaded video.
  name: status
  type: object
- description: Statistics about the video such as the number of times the video has been viewed or liked.
  name: statistics
  type: object
- description: Information used to play the video.
  name: player
  type: object
- description: The localizations object contains translations of the video's metadata.
  name: localizations
  type: object
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-video-schema.json
slug: youtube-data-video
source_filename: youtube-data-video-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A video resource represents a YouTube video.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#video.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID that YouTube uses to uniquely identify the video.\",\n      \"example\": \"abc123def456\"\n    },\n    \"snippet\": {\n      \"type\": \"object\",\n      \"description\": \"Basic details about a video, including its title, description, tags, and category.\",\n      \"properties\": {\n        \"publishedAt\": {\n          \"type\": \"string\",\n          \"description\": \"The date and time when the video was published.\",\n          \"example\":\
  \ \"2026-01-15T10:30:00Z\",\n          \"format\": \"date-time\"\n        },\n        \"channelId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the YouTube channel that published the video.\",\n          \"example\": \"500123\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The video title.\",\n          \"example\": \"Example Title\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The video description.\",\n          \"example\": \"A sample description for this resource.\"\n        },\n        \"thumbnails\": {\n          \"type\": \"object\",\n          \"description\": \"A map of thumbnail images associated with the video.\",\n          \"example\": \"example_value\"\n        },\n        \"channelTitle\": {\n          \"type\": \"string\",\n          \"description\": \"The channel title of the YouTube channel that published the video.\",\n        \
  \  \"example\": \"example_value\"\n        },\n        \"tags\": {\n          \"type\": \"array\",\n          \"description\": \"A list of keyword tags associated with the video.\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"categoryId\": {\n          \"type\": \"string\",\n          \"description\": \"The YouTube video category associated with the video.\",\n          \"example\": \"500123\"\n        },\n        \"liveBroadcastContent\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates if the video is an upcoming/active live broadcast.\",\n          \"example\": \"live\",\n          \"enum\": [\n            \"live\",\n            \"none\",\n            \"upcoming\"\n          ]\n        },\n        \"defaultLanguage\": {\n          \"type\": \"string\",\n          \"description\": \"The language of the text in the video resource's snippet.title and snippet.description properties.\"\
  ,\n          \"example\": \"en\"\n        },\n        \"localized\": {\n          \"type\": \"object\",\n          \"description\": \"The snippet.localized object contains either a localized title and description for the video or the title in the default language.\",\n          \"example\": \"example_value\",\n          \"properties\": {\n            \"title\": {\n              \"type\": \"string\",\n              \"description\": \"The localized video title.\"\n            },\n            \"description\": {\n              \"type\": \"string\",\n              \"description\": \"The localized video description.\"\n            }\n          }\n        }\n      }\n    },\n    \"contentDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the video content, including the length of the video and an indication of whether captions are available.\",\n      \"properties\": {\n        \"duration\": {\n          \"type\": \"string\",\n          \"description\": \"The\
  \ length of the video in ISO 8601 format.\",\n          \"example\": \"example_value\"\n        },\n        \"dimension\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates whether the video is available in 3D or in 2D.\",\n          \"example\": \"example_value\"\n        },\n        \"definition\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates whether the video is available in high definition or standard definition.\",\n          \"example\": \"hd\",\n          \"enum\": [\n            \"hd\",\n            \"sd\"\n          ]\n        },\n        \"caption\": {\n          \"type\": \"string\",\n          \"description\": \"Indicates whether captions are available for the video.\",\n          \"example\": \"false\",\n          \"enum\": [\n            \"false\",\n            \"true\"\n          ]\n        },\n        \"licensedContent\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether the video represents\
  \ licensed content, which means that the content has been claimed by a YouTube content partner.\",\n          \"example\": true\n        },\n        \"contentRating\": {\n          \"type\": \"object\",\n          \"description\": \"Specifies the ratings that the video received under various rating schemes.\",\n          \"example\": \"example_value\"\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"description\": \"The status of an uploaded video.\",\n      \"properties\": {\n        \"uploadStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the uploaded video.\",\n          \"example\": \"deleted\",\n          \"enum\": [\n            \"deleted\",\n            \"failed\",\n            \"processed\",\n            \"rejected\",\n            \"uploaded\"\n          ]\n        },\n        \"privacyStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The video's privacy status.\",\n          \"\
  example\": \"private\",\n          \"enum\": [\n            \"private\",\n            \"public\",\n            \"unlisted\"\n          ]\n        },\n        \"license\": {\n          \"type\": \"string\",\n          \"description\": \"The video's license.\",\n          \"example\": \"creativeCommon\",\n          \"enum\": [\n            \"creativeCommon\",\n            \"youtube\"\n          ]\n        },\n        \"embeddable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether the video can be embedded on another website.\",\n          \"example\": true\n        },\n        \"publicStatsViewable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether the video's extended statistics on the video's watch page are publicly viewable.\",\n          \"example\": true\n        },\n        \"madeForKids\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether the video is designated as child-directed.\"\
  ,\n          \"example\": \"channel==UC_x5XG1OV2P6uZZ5FSM9Ttw\"\n        }\n      }\n    },\n    \"statistics\": {\n      \"type\": \"object\",\n      \"description\": \"Statistics about the video such as the number of times the video has been viewed or liked.\",\n      \"properties\": {\n        \"viewCount\": {\n          \"type\": \"string\",\n          \"description\": \"The number of times the video has been viewed.\",\n          \"example\": 42\n        },\n        \"likeCount\": {\n          \"type\": \"string\",\n          \"description\": \"The number of users who have indicated that they liked the video.\",\n          \"example\": 42\n        },\n        \"dislikeCount\": {\n          \"type\": \"string\",\n          \"description\": \"The number of users who have indicated that they disliked the video.\",\n          \"example\": 42\n        },\n        \"favoriteCount\": {\n          \"type\": \"string\",\n          \"description\": \"The number of users who have added the video\
  \ to their favorites list.\",\n          \"example\": 42\n        },\n        \"commentCount\": {\n          \"type\": \"string\",\n          \"description\": \"The number of comments for the video.\",\n          \"example\": 42\n        }\n      }\n    },\n    \"player\": {\n      \"type\": \"object\",\n      \"description\": \"Information used to play the video.\",\n      \"properties\": {\n        \"embedHtml\": {\n          \"type\": \"string\",\n          \"description\": \"An iframe tag that embeds a player that will play the video.\",\n          \"example\": \"example_value\"\n        },\n        \"embedHeight\": {\n          \"type\": \"number\",\n          \"description\": \"The height of the embedded player returned in the player.embedHtml property.\",\n          \"example\": 42.5\n        },\n        \"embedWidth\": {\n          \"type\": \"number\",\n          \"description\": \"The width of the embedded player returned in the player.embedHtml property.\",\n          \"example\"\
  : 42.5\n        }\n      }\n    },\n    \"localizations\": {\n      \"type\": \"object\",\n      \"description\": \"The localizations object contains translations of the video's metadata.\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"kind\",\n    \"etag\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Video\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-video-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: Video
---
