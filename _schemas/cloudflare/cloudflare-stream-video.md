---
description: ''
layout: schema
name: Video
properties_list:
- description: The unique identifier of the video.
  name: uid
  type: string
- description: URL of the video thumbnail.
  name: thumbnail
  type: string
- description: ''
  name: playback
  type: object
- description: ''
  name: status
  type: object
- description: User-defined metadata.
  name: meta
  type: object
- description: ''
  name: created
  type: string
- description: ''
  name: modified
  type: string
- description: Duration of the video in seconds.
  name: duration
  type: number
- description: Size of the video in bytes.
  name: size
  type: integer
- description: ''
  name: requireSignedURLs
  type: boolean
- description: ''
  name: allowedOrigins
  type: array
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-stream-video-schema.json
slug: cloudflare-stream-video
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Video\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uid\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the video.\"\n    },\n    \"thumbnail\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the video thumbnail.\"\n    },\n    \"playback\": {\n      \"type\": \"object\"\n    },\n    \"status\": {\n      \"type\": \"object\"\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"description\": \"User-defined metadata.\"\n    },\n    \"created\": {\n      \"type\": \"string\"\n    },\n    \"modified\": {\n      \"type\": \"string\"\n    },\n    \"duration\": {\n      \"type\": \"number\",\n      \"description\": \"Duration of the video in seconds.\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the video in bytes.\"\n    },\n    \"requireSignedURLs\": {\n      \"type\": \"boolean\"\
  \n    },\n    \"allowedOrigins\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-stream-video-schema.json
tags:
- AI Gateway
- API Gateway
- Artificial Intelligence
- CDN
- Cloud
- Containers
- DDoS Protection
- DNS
- Edge
- Edge Computing
- Object Storage
- Platform
- Real-Time Communication
- Security
- Serverless
- Web Performance
title: Video
---
