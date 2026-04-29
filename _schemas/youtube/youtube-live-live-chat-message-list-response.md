---
description: A list of live chat message resources for a given broadcast.
layout: schema
name: LiveChatMessageListResponse
properties_list:
- description: Identifies the API resource's type. Value is youtube#liveChatMessageListResponse.
  name: kind
  type: string
- description: The Etag of this resource.
  name: etag
  type: string
- description: The token for the next page of results.
  name: nextPageToken
  type: string
- description: The amount of time the client should wait before polling again, in milliseconds.
  name: pollingIntervalMillis
  type: integer
- description: The date and time when the underlying stream went offline.
  name: offlineAt
  type: string
- description: Paging details for a list of live streaming resources.
  name: pageInfo
  type: object
- description: A list of chat messages that match the request criteria.
  name: items
  type: array
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-live-live-chat-message-list-response-schema.json
slug: youtube-live-live-chat-message-list-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A list of live chat message resources for a given broadcast.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#liveChatMessageListResponse.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"nextPageToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token for the next page of results.\",\n      \"example\": \"eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9\"\n    },\n    \"pollingIntervalMillis\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of time the client should wait before polling again, in milliseconds.\",\n      \"example\": 10\n    },\n    \"offlineAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time\
  \ when the underlying stream went offline.\",\n      \"example\": \"2026-01-15T10:30:00Z\",\n      \"format\": \"date-time\"\n    },\n    \"pageInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Paging details for a list of live streaming resources.\",\n      \"properties\": {\n        \"totalResults\": {\n          \"type\": \"integer\",\n          \"description\": \"The total number of results in the result set.\",\n          \"example\": 42\n        },\n        \"resultsPerPage\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of results included in the API response.\",\n          \"example\": 10\n        }\n      }\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"A list of chat messages that match the request criteria.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A liveChatMessage resource represents a chat message in a YouTube live broadcast.\",\n\
  \        \"properties\": {\n          \"kind\": {\n            \"type\": \"string\",\n            \"description\": \"Identifies the API resource's type. Value is youtube#liveChatMessage.\",\n            \"example\": \"youtube#video\"\n          },\n          \"etag\": {\n            \"type\": \"string\",\n            \"description\": \"The Etag of this resource.\",\n            \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The ID that YouTube assigns to uniquely identify the message.\",\n            \"example\": \"abc123def456\"\n          },\n          \"snippet\": {\n            \"type\": \"object\",\n            \"description\": \"The snippet object contains basic details about the message.\",\n            \"example\": \"example_value\",\n            \"properties\": {\n              \"liveChatId\": {\n                \"type\": \"string\",\n                \"description\": \"The ID of\
  \ the live chat to which this message belongs.\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"The type of message.\",\n                \"enum\": [\n                  \"chatEndedEvent\",\n                  \"fanFundingEvent\",\n                  \"giftMembershipReceivedEvent\",\n                  \"memberMilestoneChatEvent\",\n                  \"membershipGiftingEvent\",\n                  \"messageDeletedEvent\",\n                  \"newSponsorEvent\",\n                  \"pollClosedEvent\",\n                  \"pollEditedEvent\",\n                  \"pollOpenedEvent\",\n                  \"pollVotedEvent\",\n                  \"sponsorOnlyModeEndedEvent\",\n                  \"sponsorOnlyModeStartedEvent\",\n                  \"superChatEvent\",\n                  \"superStickerEvent\",\n                  \"textMessageEvent\",\n                  \"tombstone\",\n                  \"userBannedEvent\"\n         \
  \       ]\n              },\n              \"displayMessage\": {\n                \"type\": \"string\",\n                \"description\": \"Contains a string that can be displayed to the user. The string is not necessarily the message text itself.\"\n              },\n              \"authorChannelId\": {\n                \"type\": \"string\",\n                \"description\": \"The ID of the user that authored this message.\"\n              },\n              \"publishedAt\": {\n                \"type\": \"string\",\n                \"description\": \"The date and time when the message was orignally published.\",\n                \"format\": \"date-time\"\n              },\n              \"hasDisplayContent\": {\n                \"type\": \"boolean\",\n                \"description\": \"Whether the message has display content that should be displayed to users.\"\n              },\n              \"textMessageDetails\": {\n                \"type\": \"object\",\n                \"description\"\
  : \"Details about the text message. This object is only present if the type is textMessageEvent.\",\n                \"properties\": {\n                  \"messageText\": {\n                    \"type\": \"string\",\n                    \"description\": \"The user's message.\"\n                  }\n                }\n              }\n            }\n          },\n          \"authorDetails\": {\n            \"type\": \"object\",\n            \"description\": \"The authorDetails object contains basic details about the user that posted this message.\",\n            \"example\": \"example_value\",\n            \"properties\": {\n              \"channelId\": {\n                \"type\": \"string\",\n                \"description\": \"The YouTube channel ID of the message author.\"\n              },\n              \"channelUrl\": {\n                \"type\": \"string\",\n                \"description\": \"The channel URL of the message author.\"\n              },\n              \"displayName\"\
  : {\n                \"type\": \"string\",\n                \"description\": \"The channel's display name.\"\n              },\n              \"profileImageUrl\": {\n                \"type\": \"string\",\n                \"description\": \"The channel's avatar URL.\"\n              },\n              \"isVerified\": {\n                \"type\": \"boolean\",\n                \"description\": \"Indicates whether YouTube has verified the authenticity of the channel owner's identity.\"\n              },\n              \"isChatOwner\": {\n                \"type\": \"boolean\",\n                \"description\": \"Indicates whether the user is the owner of the live chat.\"\n              },\n              \"isChatSponsor\": {\n                \"type\": \"boolean\",\n                \"description\": \"Indicates whether the user is a sponsor of the live chat.\"\n              },\n              \"isChatModerator\": {\n                \"type\": \"boolean\",\n                \"description\": \"Indicates\
  \ whether the user is a moderator of the live chat.\"\n              }\n            }\n          }\n        },\n        \"required\": [\n          \"kind\",\n          \"etag\"\n        ]\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LiveChatMessageListResponse\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-live-streaming-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-live-live-chat-message-list-response-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: LiveChatMessageListResponse
---
