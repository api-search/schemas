---
description: A list of playlist item resources matching the request criteria.
layout: schema
name: PlaylistItemListResponse
properties_list:
- description: Identifies the API resource's type. Value is youtube#playlistItemListResponse.
  name: kind
  type: string
- description: The Etag of this resource.
  name: etag
  type: string
- description: The token for the next page of results.
  name: nextPageToken
  type: string
- description: The token for the previous page of results.
  name: prevPageToken
  type: string
- description: Paging details for a list operation, including information about the total number of resources and the number per page.
  name: pageInfo
  type: object
- description: A list of playlist items that match the request criteria.
  name: items
  type: array
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-playlist-item-list-response-schema.json
slug: youtube-data-playlist-item-list-response
source_filename: youtube-data-playlist-item-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A list of playlist item resources matching the request criteria.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#playlistItemListResponse.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token for the next page of results.\",\n      \"example\": \"eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9\"\n    },\n    \"prevPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token for the previous page of results.\",\n      \"example\": \"eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9\"\n    },\n    \"pageInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Paging details for a list\
  \ operation, including information about the total number of resources and the number per page.\",\n      \"properties\": {\n        \"totalResults\": {\n          \"type\": \"integer\",\n          \"description\": \"The total number of results in the result set.\",\n          \"example\": 42\n        },\n        \"resultsPerPage\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of results included in the API response.\",\n          \"example\": 10\n        }\n      }\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"A list of playlist items that match the request criteria.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A playlistItem resource identifies another resource, such as a video, that is included in a playlist.\",\n        \"properties\": {\n          \"kind\": {\n            \"type\": \"string\",\n            \"description\": \"Identifies the API resource's type.\
  \ Value is youtube#playlistItem.\",\n            \"example\": \"youtube#video\"\n          },\n          \"etag\": {\n            \"type\": \"string\",\n            \"description\": \"The Etag of this resource.\",\n            \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The ID that YouTube uses to uniquely identify the playlist item.\",\n            \"example\": \"abc123def456\"\n          },\n          \"snippet\": {\n            \"type\": \"object\",\n            \"description\": \"Basic details about the playlist item such as its title and position in the playlist.\",\n            \"example\": \"example_value\",\n            \"properties\": {\n              \"publishedAt\": {\n                \"type\": \"string\",\n                \"description\": \"The date and time that the item was added to the playlist.\",\n                \"format\": \"date-time\"\n              },\n         \
  \     \"channelId\": {\n                \"type\": \"string\",\n                \"description\": \"The ID of the user that added the video to the playlist.\"\n              },\n              \"title\": {\n                \"type\": \"string\",\n                \"description\": \"The item title.\"\n              },\n              \"description\": {\n                \"type\": \"string\",\n                \"description\": \"The item description.\"\n              },\n              \"thumbnails\": {\n                \"type\": \"object\",\n                \"description\": \"A map of thumbnail images associated with the playlist item.\"\n              },\n              \"channelTitle\": {\n                \"type\": \"string\",\n                \"description\": \"The channel title of the channel that the playlist item belongs to.\"\n              },\n              \"playlistId\": {\n                \"type\": \"string\",\n                \"description\": \"The ID of the playlist that the playlist\
  \ item is in.\"\n              },\n              \"position\": {\n                \"type\": \"integer\",\n                \"description\": \"The order in which the item appears in the playlist.\"\n              },\n              \"resourceId\": {\n                \"type\": \"object\",\n                \"description\": \"The id object contains information that can be used to uniquely identify the resource that is included in the playlist as the playlist item.\",\n                \"properties\": {\n                  \"kind\": {\n                    \"type\": \"string\",\n                    \"description\": \"The kind, or type, of the referred resource.\"\n                  },\n                  \"videoId\": {\n                    \"type\": \"string\",\n                    \"description\": \"If the snippet.resourceId.kind property has a value of youtube#video, this property is present.\"\n                  }\n                }\n              }\n            }\n          },\n          \"contentDetails\"\
  : {\n            \"type\": \"object\",\n            \"description\": \"The contentDetails object is included in the resource if the included item is a YouTube video.\",\n            \"example\": \"example_value\",\n            \"properties\": {\n              \"videoId\": {\n                \"type\": \"string\",\n                \"description\": \"The ID that YouTube uses to uniquely identify a video.\"\n              },\n              \"videoPublishedAt\": {\n                \"type\": \"string\",\n                \"description\": \"The date and time that the video was published to YouTube.\",\n                \"format\": \"date-time\"\n              }\n            }\n          },\n          \"status\": {\n            \"type\": \"object\",\n            \"description\": \"The status object contains information about the playlist item's privacy status.\",\n            \"example\": \"example_value\",\n            \"properties\": {\n              \"privacyStatus\": {\n                \"type\"\
  : \"string\",\n                \"description\": \"The playlist item's privacy status.\"\n              }\n            }\n          }\n        },\n        \"required\": [\n          \"kind\",\n          \"etag\"\n        ]\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PlaylistItemListResponse\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-playlist-item-list-response-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: PlaylistItemListResponse
---
