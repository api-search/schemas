---
description: A comment resource contains information about a single YouTube comment.
layout: schema
name: Comment
properties_list:
- description: Identifies the API resource's type. Value is youtube#comment.
  name: kind
  type: string
- description: The Etag of this resource.
  name: etag
  type: string
- description: The ID that YouTube uses to uniquely identify the comment.
  name: id
  type: string
- description: The snippet object contains basic details about the comment.
  name: snippet
  type: object
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-comment-schema.json
slug: youtube-data-comment
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A comment resource contains information about a single YouTube comment.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#comment.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID that YouTube uses to uniquely identify the comment.\",\n      \"example\": \"abc123def456\"\n    },\n    \"snippet\": {\n      \"type\": \"object\",\n      \"description\": \"The snippet object contains basic details about the comment.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"textOriginal\": {\n          \"type\": \"string\",\n          \"description\": \"The original text of the comment\
  \ as it was initially posted.\"\n        },\n        \"textDisplay\": {\n          \"type\": \"string\",\n          \"description\": \"The comment text as displayed to users.\"\n        },\n        \"authorDisplayName\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the user who posted the comment.\"\n        },\n        \"authorProfileImageUrl\": {\n          \"type\": \"string\",\n          \"description\": \"The URL for the avatar of the user who posted the comment.\"\n        },\n        \"authorChannelUrl\": {\n          \"type\": \"string\",\n          \"description\": \"A link to the YouTube channel of the comment's author.\"\n        },\n        \"authorChannelId\": {\n          \"type\": \"object\",\n          \"description\": \"An object that encapsulates information about the comment author's YouTube channel.\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"string\",\n              \"description\": \"\
  The author's YouTube channel ID.\"\n            }\n          }\n        },\n        \"likeCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The total number of likes that the comment has received.\"\n        },\n        \"viewerRating\": {\n          \"type\": \"string\",\n          \"description\": \"The rating the viewer has given to this comment. Note that this property does not currently identify dislike ratings.\"\n        },\n        \"publishedAt\": {\n          \"type\": \"string\",\n          \"description\": \"The date and time when the comment was originally published.\",\n          \"format\": \"date-time\"\n        },\n        \"updatedAt\": {\n          \"type\": \"string\",\n          \"description\": \"The date and time when the comment was last updated.\",\n          \"format\": \"date-time\"\n        },\n        \"videoId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the video the comment refers to.\"\n        },\n\
  \        \"parentId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique ID of the parent comment.\"\n        },\n        \"canRate\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether the current viewer can rate the comment.\"\n        },\n        \"moderationStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The comment's moderation status.\",\n          \"enum\": [\n            \"heldForReview\",\n            \"likelySpam\",\n            \"published\",\n            \"rejected\"\n          ]\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"kind\",\n    \"etag\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Comment\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-comment-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: Comment
---
