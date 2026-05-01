---
description: StreamKeyArnList schema
layout: schema
name: StreamKeyArnList
properties_list: []
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-stream-key-arn-list-schema.json
slug: ivs-stream-key-arn-list
source_filename: ivs-stream-key-arn-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stream-key-arn-list-schema.json\",\n  \"title\": \"StreamKeyArnList\",\n  \"description\": \"StreamKeyArnList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"^arn:aws:[is]vs:[a-z0-9-]+:[0-9]+:stream-key/[a-zA-Z0-9-]+$\",\n    \"minLength\": 1,\n    \"maxLength\": 128\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stream-key-arn-list-schema.json
tags:
- Live Streaming
- Media
- Video
- Real-Time
title: StreamKeyArnList
---
