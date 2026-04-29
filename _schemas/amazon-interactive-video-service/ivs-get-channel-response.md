---
description: GetChannelResponse schema
layout: schema
name: GetChannelResponse
properties_list:
- description: ''
  name: channel
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-get-channel-response-schema.json
slug: ivs-get-channel-response
source_filename: ivs-get-channel-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-channel-response-schema.json\",\n  \"title\": \"GetChannelResponse\",\n  \"description\": \"GetChannelResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Channel\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-channel-response-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: GetChannelResponse
---
