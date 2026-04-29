---
description: Describes the content of a YouTube Analytics group in terms of the number of items it contains and the type of items it contains.
layout: schema
name: GroupContentDetails
properties_list:
- description: The number of items in the group.
  name: itemCount
  type: integer
- description: The type of resources contained in the group. Valid values are youtube#channel, youtube#playlist, youtube#video, and youtubePartner#asset.
  name: itemType
  type: string
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-analytics-group-content-details-schema.json
slug: youtube-analytics-group-content-details
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Describes the content of a YouTube Analytics group in terms of the number of items it contains and the type of items it contains.\",\n  \"properties\": {\n    \"itemCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items in the group.\",\n      \"example\": 42,\n      \"format\": \"int64\"\n    },\n    \"itemType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of resources contained in the group. Valid values are youtube#channel, youtube#playlist, youtube#video, and youtubePartner#asset.\",\n      \"example\": \"youtube#channel\",\n      \"enum\": [\n        \"youtube#channel\",\n        \"youtube#playlist\",\n        \"youtube#video\",\n        \"youtubePartner#asset\"\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupContentDetails\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-analytics-openapi.yml\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-analytics-group-content-details-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: GroupContentDetails
---
