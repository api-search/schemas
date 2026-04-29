---
description: A list of caption resources associated with the specified video.
layout: schema
name: CaptionListResponse
properties_list:
- description: Identifies the API resource's type. Value is youtube#captionListResponse.
  name: kind
  type: string
- description: The Etag of this resource.
  name: etag
  type: string
- description: A list of captions that match the request criteria.
  name: items
  type: array
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-caption-list-response-schema.json
slug: youtube-data-caption-list-response
source_filename: youtube-data-caption-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A list of caption resources associated with the specified video.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies the API resource's type. Value is youtube#captionListResponse.\",\n      \"example\": \"youtube#video\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The Etag of this resource.\",\n      \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"A list of captions that match the request criteria.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A caption resource represents a YouTube caption track. A caption track is associated with exactly one YouTube video.\",\n        \"properties\": {\n          \"kind\": {\n            \"type\": \"string\",\n            \"description\": \"Identifies the API resource's\
  \ type. Value is youtube#caption.\",\n            \"example\": \"youtube#video\"\n          },\n          \"etag\": {\n            \"type\": \"string\",\n            \"description\": \"The Etag of this resource.\",\n            \"example\": \"XI7nbFXulYBIpL0ayR_gDh3eu1k\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The ID that YouTube uses to uniquely identify the caption track.\",\n            \"example\": \"abc123def456\"\n          },\n          \"snippet\": {\n            \"type\": \"object\",\n            \"description\": \"The snippet object contains basic details about the caption.\",\n            \"example\": \"example_value\",\n            \"properties\": {\n              \"videoId\": {\n                \"type\": \"string\",\n                \"description\": \"The ID of the video that the caption track is associated with.\"\n              },\n              \"lastUpdated\": {\n                \"type\": \"string\",\n    \
  \            \"description\": \"The date and time when the caption track was last updated.\",\n                \"format\": \"date-time\"\n              },\n              \"trackKind\": {\n                \"type\": \"string\",\n                \"description\": \"The caption track's type.\",\n                \"enum\": [\n                  \"asr\",\n                  \"forced\",\n                  \"standard\"\n                ]\n              },\n              \"language\": {\n                \"type\": \"string\",\n                \"description\": \"The language of the caption track. The property value is a BCP-47 language tag.\"\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"The name of the caption track.\"\n              },\n              \"audioTrackType\": {\n                \"type\": \"string\",\n                \"description\": \"The type of audio track associated with the caption track.\",\n                \"\
  enum\": [\n                  \"commentary\",\n                  \"descriptive\",\n                  \"primary\",\n                  \"unknown\"\n                ]\n              },\n              \"isCC\": {\n                \"type\": \"boolean\",\n                \"description\": \"Indicates whether the track contains closed captions for the deaf and hard of hearing.\"\n              },\n              \"isLarge\": {\n                \"type\": \"boolean\",\n                \"description\": \"Indicates whether the caption track uses large text for the vision-impaired.\"\n              },\n              \"isEasyReader\": {\n                \"type\": \"boolean\",\n                \"description\": \"Indicates whether caption track is formatted for easy reader.\"\n              },\n              \"isDraft\": {\n                \"type\": \"boolean\",\n                \"description\": \"Indicates whether the caption track is a draft.\"\n              },\n              \"isAutoSynced\": {\n  \
  \              \"type\": \"boolean\",\n                \"description\": \"Indicates whether YouTube synchronized the caption track to the audio track in the video.\"\n              },\n              \"status\": {\n                \"type\": \"string\",\n                \"description\": \"The caption track's status.\",\n                \"enum\": [\n                  \"failed\",\n                  \"serving\",\n                  \"syncing\"\n                ]\n              }\n            }\n          }\n        },\n        \"required\": [\n          \"kind\",\n          \"etag\"\n        ]\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CaptionListResponse\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-caption-list-response-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: CaptionListResponse
---
