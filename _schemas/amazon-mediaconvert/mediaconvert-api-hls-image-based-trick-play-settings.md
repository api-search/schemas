---
description: Tile and thumbnail settings applicable when imageBasedTrickPlay is ADVANCED
layout: schema
name: HlsImageBasedTrickPlaySettings
properties_list:
- description: ''
  name: IntervalCadence
  type: object
- description: ''
  name: ThumbnailHeight
  type: object
- description: ''
  name: ThumbnailInterval
  type: object
- description: ''
  name: ThumbnailWidth
  type: object
- description: ''
  name: TileHeight
  type: object
- description: ''
  name: TileWidth
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-image-based-trick-play-settings-schema.json
slug: mediaconvert-api-hls-image-based-trick-play-settings
source_filename: mediaconvert-api-hls-image-based-trick-play-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-image-based-trick-play-settings-schema.json\",\n  \"title\": \"HlsImageBasedTrickPlaySettings\",\n  \"description\": \"Tile and thumbnail settings applicable when imageBasedTrickPlay is ADVANCED\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IntervalCadence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsIntervalCadence\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"intervalCadence\"\n          },\n          \"description\": \"The cadence MediaConvert follows for generating thumbnails. If set to FOLLOW_IFRAME, MediaConvert generates thumbnails for each IDR frame in the output (matching the GOP cadence). If set to FOLLOW_CUSTOM, MediaConvert generates thumbnails according to the interval you specify in thumbnailInterval.\"\
  \n        }\n      ]\n    },\n    \"ThumbnailHeight\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin2Max4096\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"thumbnailHeight\"\n          },\n          \"description\": \"Height of each thumbnail within each tile image, in pixels. Leave blank to maintain aspect ratio with thumbnail width. If following the aspect ratio would lead to a total tile height greater than 4096, then the job will be rejected. Must be divisible by 2.\"\n        }\n      ]\n    },\n    \"ThumbnailInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"thumbnailInterval\"\n          },\n          \"description\": \"Enter the interval, in seconds, that MediaConvert uses to generate thumbnails. If the interval you enter doesn't align with the output frame rate, MediaConvert\
  \ automatically rounds the interval to align with the output frame rate. For example, if the output frame rate is 29.97 frames per second and you enter 5, MediaConvert uses a 150 frame interval to generate thumbnails.\"\n        }\n      ]\n    },\n    \"ThumbnailWidth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin8Max4096\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"thumbnailWidth\"\n          },\n          \"description\": \"Width of each thumbnail within each tile image, in pixels. Default is 312. Must be divisible by 8.\"\n        }\n      ]\n    },\n    \"TileHeight\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2048\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tileHeight\"\n          },\n          \"description\": \"Number of thumbnails in each column of a tile image. Set a value between 2 and 2048. Must be divisible by 2.\"\n      \
  \  }\n      ]\n    },\n    \"TileWidth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max512\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tileWidth\"\n          },\n          \"description\": \"Number of thumbnails in each row of a tile image. Set a value between 1 and 512.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-image-based-trick-play-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: HlsImageBasedTrickPlaySettings
---
