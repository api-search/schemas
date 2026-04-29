---
description: The status of an uploaded video.
layout: schema
name: VideoStatus
properties_list:
- description: The status of the uploaded video.
  name: uploadStatus
  type: string
- description: The video's privacy status.
  name: privacyStatus
  type: string
- description: The video's license.
  name: license
  type: string
- description: Indicates whether the video can be embedded on another website.
  name: embeddable
  type: boolean
- description: Indicates whether the video's extended statistics on the video's watch page are publicly viewable.
  name: publicStatsViewable
  type: boolean
- description: Indicates whether the video is designated as child-directed.
  name: madeForKids
  type: boolean
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-video-status-schema.json
slug: youtube-data-video-status
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The status of an uploaded video.\",\n  \"properties\": {\n    \"uploadStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the uploaded video.\",\n      \"example\": \"deleted\",\n      \"enum\": [\n        \"deleted\",\n        \"failed\",\n        \"processed\",\n        \"rejected\",\n        \"uploaded\"\n      ]\n    },\n    \"privacyStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The video's privacy status.\",\n      \"example\": \"private\",\n      \"enum\": [\n        \"private\",\n        \"public\",\n        \"unlisted\"\n      ]\n    },\n    \"license\": {\n      \"type\": \"string\",\n      \"description\": \"The video's license.\",\n      \"example\": \"creativeCommon\",\n      \"enum\": [\n        \"creativeCommon\",\n        \"youtube\"\n      ]\n    },\n    \"embeddable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the video can be\
  \ embedded on another website.\",\n      \"example\": true\n    },\n    \"publicStatsViewable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the video's extended statistics on the video's watch page are publicly viewable.\",\n      \"example\": true\n    },\n    \"madeForKids\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the video is designated as child-directed.\",\n      \"example\": \"channel==UC_x5XG1OV2P6uZZ5FSM9Ttw\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VideoStatus\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-video-status-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: VideoStatus
---
