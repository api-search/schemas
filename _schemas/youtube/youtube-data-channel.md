---
description: A channel resource represents a YouTube channel.
layout: schema
name: Channel
properties_list:
- description: Identifies the API resource's type. Value is youtube#channel.
  name: kind
  type: string
- description: The Etag of this resource.
  name: etag
  type: string
- description: The ID that YouTube uses to uniquely identify the channel.
  name: id
  type: string
- description: Basic details about a channel, including its title, description, and thumbnails.
  name: snippet
  type: object
- description: Statistics about a YouTube channel.
  name: statistics
  type: object
- description: The contentDetails object encapsulates information about the channel's content.
  name: contentDetails
  type: object
- description: The brandingSettings object encapsulates information about the branding of the channel.
  name: brandingSettings
  type: object
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-channel-schema.json
slug: youtube-data-channel
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A channel resource represents a YouTube channel.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#channel.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID that YouTube uses to uniquely identify the channel.\",\n      \"example\": \"abc123def456\"\n    },\n    \"snippet\": {\n      \"type\": \"object\",\n      \"description\": \"Basic details about a channel, including its title, description, and thumbnails.\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The channel title.\",\n          \"example\": \"Example Title\"\n        },\n\
  \        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The channel description.\",\n          \"example\": \"A sample description for this resource.\"\n        },\n        \"customUrl\": {\n          \"type\": \"string\",\n          \"description\": \"The channel's custom URL.\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"publishedAt\": {\n          \"type\": \"string\",\n          \"description\": \"The date and time that the channel was created.\",\n          \"example\": \"2026-01-15T10:30:00Z\",\n          \"format\": \"date-time\"\n        },\n        \"thumbnails\": {\n          \"type\": \"object\",\n          \"description\": \"A map of thumbnail images associated with the channel.\",\n          \"example\": \"example_value\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"The country with which the channel is associated.\",\n          \"example\": 42\n       \
  \ },\n        \"localized\": {\n          \"type\": \"object\",\n          \"description\": \"The snippet.localized object contains a localized title and description for the channel.\",\n          \"example\": \"example_value\",\n          \"properties\": {\n            \"title\": {\n              \"type\": \"string\",\n              \"description\": \"The localized channel title.\"\n            },\n            \"description\": {\n              \"type\": \"string\",\n              \"description\": \"The localized channel description.\"\n            }\n          }\n        }\n      }\n    },\n    \"statistics\": {\n      \"type\": \"object\",\n      \"description\": \"Statistics about a YouTube channel.\",\n      \"properties\": {\n        \"viewCount\": {\n          \"type\": \"string\",\n          \"description\": \"The number of times the channel has been viewed.\",\n          \"example\": 42\n        },\n        \"subscriberCount\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The number of subscribers that the channel has.\",\n          \"example\": 42\n        },\n        \"hiddenSubscriberCount\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether the channel's subscriber count is publicly visible.\",\n          \"example\": 42\n        },\n        \"videoCount\": {\n          \"type\": \"string\",\n          \"description\": \"The number of public videos uploaded to the channel.\",\n          \"example\": 42\n        }\n      }\n    },\n    \"contentDetails\": {\n      \"type\": \"object\",\n      \"description\": \"The contentDetails object encapsulates information about the channel's content.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"relatedPlaylists\": {\n          \"type\": \"object\",\n          \"description\": \"A map that identifies playlists associated with the channel.\",\n          \"properties\": {\n            \"uploads\": {\n              \"type\": \"string\",\n      \
  \        \"description\": \"The ID of the playlist that contains the channel's uploaded videos.\"\n            },\n            \"likes\": {\n              \"type\": \"string\",\n              \"description\": \"The ID of the playlist that contains the videos that the channel has liked.\"\n            }\n          }\n        }\n      }\n    },\n    \"brandingSettings\": {\n      \"type\": \"object\",\n      \"description\": \"The brandingSettings object encapsulates information about the branding of the channel.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"channel\": {\n          \"type\": \"object\",\n          \"description\": \"Branding settings for the channel page.\",\n          \"properties\": {\n            \"title\": {\n              \"type\": \"string\",\n              \"description\": \"The channel title.\"\n            },\n            \"description\": {\n              \"type\": \"string\",\n              \"description\": \"The channel description.\"\
  \n            },\n            \"keywords\": {\n              \"type\": \"string\",\n              \"description\": \"Keywords associated with the channel.\"\n            },\n            \"defaultLanguage\": {\n              \"type\": \"string\",\n              \"description\": \"The content tab that users should display by default on the channel page.\"\n            }\n          }\n        },\n        \"image\": {\n          \"type\": \"object\",\n          \"description\": \"Branding images associated with the channel page.\",\n          \"properties\": {\n            \"bannerExternalUrl\": {\n              \"type\": \"string\",\n              \"description\": \"The URL for the banner image shown on the channel page on the YouTube website.\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"kind\",\n    \"etag\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Channel\",\n  \"x-schema-source\": \"openapi\",\n\
  \  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-channel-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: Channel
---
