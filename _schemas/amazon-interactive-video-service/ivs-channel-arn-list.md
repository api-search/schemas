---
description: ChannelArnList schema
layout: schema
name: ChannelArnList
properties_list: []
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-channel-arn-list-schema.json
slug: ivs-channel-arn-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-channel-arn-list-schema.json\",\n  \"title\": \"ChannelArnList\",\n  \"description\": \"ChannelArnList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"pattern\": \"^arn:aws:[is]vs:[a-z0-9-]+:[0-9]+:channel/[a-zA-Z0-9-]+$\",\n    \"minLength\": 1,\n    \"maxLength\": 128\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-channel-arn-list-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: ChannelArnList
---
