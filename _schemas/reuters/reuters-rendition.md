---
description: A specific rendition or format of a media item from the Reuters Connect API. Renditions represent different sizes, resolutions, or formats of the same content available for download. Images may have thumbnail, preview, and full-size renditions, while video may have different quality levels and formats.
layout: schema
name: Reuters Connect Rendition
properties_list:
- description: The name or label of the rendition indicating its purpose or size class.
  name: name
  type: string
- description: The URL to download this rendition of the content. Requires a valid authentication token to access.
  name: href
  type: string
- description: The MIME type of the rendition file, indicating the file format.
  name: mimetype
  type: string
- description: The width of the rendition in pixels. Applicable to image and video renditions.
  name: width
  type: integer
- description: The height of the rendition in pixels. Applicable to image and video renditions.
  name: height
  type: integer
- description: The file size of the rendition in bytes.
  name: sizeinbytes
  type: integer
- description: The duration of the rendition in seconds. Applicable to video and audio renditions.
  name: duration
  type: number
- description: The specific format or codec of the rendition, providing additional detail beyond the MIME type.
  name: format
  type: string
provider_name: Reuters
provider_slug: reuters
schema_file: json-schema/reuters-rendition-schema.json
slug: reuters-rendition
source_filename: reuters-rendition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/kinlane/reuters/json-schema/reuters-rendition-schema.json\",\n  \"title\": \"Reuters Connect Rendition\",\n  \"description\": \"A specific rendition or format of a media item from the Reuters Connect API. Renditions represent different sizes, resolutions, or formats of the same content available for download. Images may have thumbnail, preview, and full-size renditions, while video may have different quality levels and formats.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"href\",\n    \"mimetype\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name or label of the rendition indicating its purpose or size class.\",\n      \"examples\": [\n        \"thumbnail\",\n        \"preview\",\n        \"baseImage\",\n        \"hires\",\n        \"videoFile\",\n        \"webReadyVideo\"\n      ]\n    },\n  \
  \  \"href\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to download this rendition of the content. Requires a valid authentication token to access.\"\n    },\n    \"mimetype\": {\n      \"type\": \"string\",\n      \"description\": \"The MIME type of the rendition file, indicating the file format.\",\n      \"examples\": [\n        \"image/jpeg\",\n        \"image/png\",\n        \"image/gif\",\n        \"video/mp4\",\n        \"video/quicktime\",\n        \"application/pdf\",\n        \"text/html\"\n      ]\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"The width of the rendition in pixels. Applicable to image and video renditions.\",\n      \"minimum\": 1,\n      \"examples\": [\n        150,\n        640,\n        1920,\n        3000\n      ]\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"The height of the rendition in pixels. Applicable to image and video renditions.\"\
  ,\n      \"minimum\": 1,\n      \"examples\": [\n        100,\n        480,\n        1080,\n        2000\n      ]\n    },\n    \"sizeinbytes\": {\n      \"type\": \"integer\",\n      \"description\": \"The file size of the rendition in bytes.\",\n      \"minimum\": 0,\n      \"examples\": [\n        15360,\n        102400,\n        5242880\n      ]\n    },\n    \"duration\": {\n      \"type\": \"number\",\n      \"description\": \"The duration of the rendition in seconds. Applicable to video and audio renditions.\",\n      \"minimum\": 0\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"The specific format or codec of the rendition, providing additional detail beyond the MIME type.\",\n      \"examples\": [\n        \"JPEG\",\n        \"PNG\",\n        \"H.264\",\n        \"MPEG-4\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reuters/refs/heads/main/json-schema/reuters-rendition-schema.json
tags:
- Business
- Finance
- Journalism
- Media
- News
- Wire Service
title: Reuters Connect Rendition
---
