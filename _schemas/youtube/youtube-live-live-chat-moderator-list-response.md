---
description: A list of live chat moderator resources for a given live chat.
layout: schema
name: LiveChatModeratorListResponse
properties_list:
- description: Identifies the API resource's type. Value is youtube#liveChatModeratorListResponse.
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
- description: Paging details for a list of live streaming resources.
  name: pageInfo
  type: object
- description: A list of moderators that match the request criteria.
  name: items
  type: array
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-live-live-chat-moderator-list-response-schema.json
slug: youtube-live-live-chat-moderator-list-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A list of live chat moderator resources for a given live chat.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#liveChatModeratorListResponse.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token for the next page of results.\",\n      \"example\": \"eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9\"\n    },\n    \"prevPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token for the previous page of results.\",\n      \"example\": \"eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9\"\n    },\n    \"pageInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Paging details for\
  \ a list of live streaming resources.\",\n      \"properties\": {\n        \"totalResults\": {\n          \"type\": \"integer\",\n          \"description\": \"The total number of results in the result set.\",\n          \"example\": 42\n        },\n        \"resultsPerPage\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of results included in the API response.\",\n          \"example\": 10\n        }\n      }\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"A list of moderators that match the request criteria.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A liveChatModerator resource identifies a user who has moderator privileges in a YouTube live chat.\",\n        \"properties\": {\n          \"kind\": {\n            \"type\": \"string\",\n            \"description\": \"Identifies the API resource's type. Value is youtube#liveChatModerator.\",\n            \"example\"\
  : \"youtube#video\"\n          },\n          \"etag\": {\n            \"type\": \"string\",\n            \"description\": \"The Etag of this resource.\",\n            \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The ID that YouTube assigns to uniquely identify the moderator.\",\n            \"example\": \"abc123def456\"\n          },\n          \"snippet\": {\n            \"type\": \"object\",\n            \"description\": \"The snippet object contains basic details about the moderator.\",\n            \"example\": \"example_value\",\n            \"properties\": {\n              \"liveChatId\": {\n                \"type\": \"string\",\n                \"description\": \"The liveChatId is the live chat id for this moderator resource.\"\n              },\n              \"moderatorDetails\": {\n                \"type\": \"object\",\n                \"description\": \"Details about the moderator.\"\
  ,\n                \"properties\": {\n                  \"channelId\": {\n                    \"type\": \"string\",\n                    \"description\": \"The YouTube channel ID of the moderator.\"\n                  },\n                  \"channelUrl\": {\n                    \"type\": \"string\",\n                    \"description\": \"The channel URL of the moderator.\"\n                  },\n                  \"displayName\": {\n                    \"type\": \"string\",\n                    \"description\": \"The channel's display name.\"\n                  },\n                  \"profileImageUrl\": {\n                    \"type\": \"string\",\n                    \"description\": \"The channel's avatar URL.\"\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"required\": [\n          \"kind\",\n          \"etag\"\n        ]\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\"\
  : \"LiveChatModeratorListResponse\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-live-streaming-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-live-live-chat-moderator-list-response-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: LiveChatModeratorListResponse
---
