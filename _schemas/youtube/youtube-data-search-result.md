---
description: A search result contains information about a YouTube video, channel, or playlist that matches the search query.
layout: schema
name: SearchResult
properties_list:
- description: Identifies the API resource's type. Value is youtube#searchResult.
  name: kind
  type: string
- description: The Etag of this resource.
  name: etag
  type: string
- description: The id object contains information that can be used to uniquely identify the resource that matches the search request.
  name: id
  type: object
- description: The snippet object contains basic details about a search result, such as its title or description.
  name: snippet
  type: object
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-search-result-schema.json
slug: youtube-data-search-result
source_filename: youtube-data-search-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A search result contains information about a YouTube video, channel, or playlist that matches the search query.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#searchResult.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"id\": {\n      \"type\": \"object\",\n      \"description\": \"The id object contains information that can be used to uniquely identify the resource that matches the search request.\",\n      \"example\": \"abc123def456\",\n      \"properties\": {\n        \"kind\": {\n          \"type\": \"string\",\n          \"description\": \"The type of the API resource.\"\n        },\n        \"videoId\": {\n          \"type\": \"string\",\n          \"\
  description\": \"If the id.kind property's value is youtube#video, then this property is present.\"\n        },\n        \"channelId\": {\n          \"type\": \"string\",\n          \"description\": \"If the id.kind property's value is youtube#channel, then this property is present.\"\n        },\n        \"playlistId\": {\n          \"type\": \"string\",\n          \"description\": \"If the id.kind property's value is youtube#playlist, then this property is present.\"\n        }\n      }\n    },\n    \"snippet\": {\n      \"type\": \"object\",\n      \"description\": \"The snippet object contains basic details about a search result, such as its title or description.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"publishedAt\": {\n          \"type\": \"string\",\n          \"description\": \"The creation date and time of the resource that the search result identifies.\",\n          \"format\": \"date-time\"\n        },\n        \"channelId\": {\n        \
  \  \"type\": \"string\",\n          \"description\": \"The value that YouTube uses to uniquely identify the channel that published the resource identified by the search result.\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The title of the search result.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the search result.\"\n        },\n        \"thumbnails\": {\n          \"type\": \"object\",\n          \"description\": \"A map of thumbnail images associated with the search result.\"\n        },\n        \"channelTitle\": {\n          \"type\": \"string\",\n          \"description\": \"The title of the channel that published the resource identified by the search result.\"\n        },\n        \"liveBroadcastContent\": {\n          \"type\": \"string\",\n          \"description\": \"An indication of whether a video or channel resource has live broadcast content.\"\
  \n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchResult\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-search-result-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: SearchResult
---
