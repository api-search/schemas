---
description: A list of group item resources in a specified group.
layout: schema
name: GroupItemListResponse
properties_list:
- description: Identifies the API resource's type. Value is youtube#groupItemListResponse.
  name: kind
  type: string
- description: The Etag of this resource.
  name: etag
  type: string
- description: A list of group items that are part of the specified group.
  name: items
  type: array
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-analytics-group-item-list-response-schema.json
slug: youtube-analytics-group-item-list-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A list of group item resources in a specified group.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#groupItemListResponse.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"A list of group items that are part of the specified group.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A groupItem resource identifies a resource, such as a video, channel, or playlist, that is part of a group. A group can contain a maximum of 500 items and only items of the same type (videos, channels, playlists, or assets).\",\n        \"properties\": {\n        \
  \  \"kind\": {\n            \"type\": \"string\",\n            \"description\": \"Identifies the API resource's type. Value is youtube#groupItem.\",\n            \"example\": \"youtube#video\"\n          },\n          \"etag\": {\n            \"type\": \"string\",\n            \"description\": \"The Etag of this resource.\",\n            \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The ID that YouTube uses to uniquely identify the groupItem resource.\",\n            \"example\": \"abc123def456\"\n          },\n          \"groupId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID that YouTube uses to uniquely identify the group that contains the item.\",\n            \"example\": \"500123\"\n          },\n          \"resource\": {\n            \"type\": \"object\",\n            \"description\": \"The resource object contains information that identifies the item\
  \ being added to the group.\",\n            \"example\": \"example_value\",\n            \"properties\": {\n              \"kind\": {\n                \"type\": \"string\",\n                \"description\": \"Identifies the type of resource being added to the group.\",\n                \"enum\": [\n                  \"youtube#channel\",\n                  \"youtube#playlist\",\n                  \"youtube#video\",\n                  \"youtubePartner#asset\"\n                ]\n              },\n              \"id\": {\n                \"type\": \"string\",\n                \"description\": \"The channel, video, playlist, or asset ID that YouTube uses to uniquely identify the item being added to the group.\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupItemListResponse\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-analytics-openapi.yml\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-analytics-group-item-list-response-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: GroupItemListResponse
---
