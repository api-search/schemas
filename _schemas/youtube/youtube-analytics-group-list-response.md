---
description: A list of group resources matching the request criteria.
layout: schema
name: GroupListResponse
properties_list:
- description: Identifies the API resource's type. Value is youtube#groupListResponse.
  name: kind
  type: string
- description: The Etag of this resource.
  name: etag
  type: string
- description: The token for the next page of results in the result set.
  name: nextPageToken
  type: string
- description: A list of groups that match the request criteria.
  name: items
  type: array
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-analytics-group-list-response-schema.json
slug: youtube-analytics-group-list-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A list of group resources matching the request criteria.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#groupListResponse.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token for the next page of results in the result set.\",\n      \"example\": \"eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"A list of groups that match the request criteria.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A group resource represents a YouTube Analytics group, which is\
  \ a custom collection of up to 500 channels, videos, playlists, or assets. You can use groups to simplify retrieving data for multiple resources.\",\n        \"properties\": {\n          \"kind\": {\n            \"type\": \"string\",\n            \"description\": \"Identifies the API resource's type. Value is youtube#group.\",\n            \"example\": \"youtube#video\"\n          },\n          \"etag\": {\n            \"type\": \"string\",\n            \"description\": \"The Etag of this resource.\",\n            \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The ID that YouTube uses to uniquely identify the group.\",\n            \"example\": \"abc123def456\"\n          },\n          \"snippet\": {\n            \"type\": \"object\",\n            \"description\": \"The snippet object contains basic details about the group.\",\n            \"example\": \"example_value\",\n            \"\
  properties\": {\n              \"publishedAt\": {\n                \"type\": \"string\",\n                \"description\": \"The date and time that the group was created.\",\n                \"format\": \"date-time\"\n              },\n              \"title\": {\n                \"type\": \"string\",\n                \"description\": \"The group title. The value must be a non-empty string.\"\n              }\n            }\n          },\n          \"contentDetails\": {\n            \"type\": \"object\",\n            \"description\": \"Describes the content of a YouTube Analytics group in terms of the number of items it contains and the type of items it contains.\",\n            \"properties\": {\n              \"itemCount\": {\n                \"type\": \"integer\",\n                \"description\": \"The number of items in the group.\",\n                \"example\": 42,\n                \"format\": \"int64\"\n              },\n              \"itemType\": {\n                \"type\": \"\
  string\",\n                \"description\": \"The type of resources contained in the group. Valid values are youtube#channel, youtube#playlist, youtube#video, and youtubePartner#asset.\",\n                \"example\": \"youtube#channel\",\n                \"enum\": [\n                  \"youtube#channel\",\n                  \"youtube#playlist\",\n                  \"youtube#video\",\n                  \"youtubePartner#asset\"\n                ]\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GroupListResponse\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-analytics-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-analytics-group-list-response-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: GroupListResponse
---
