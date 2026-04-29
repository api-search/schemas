---
description: ListChannelsResponse schema
layout: schema
name: ListChannelsResponse
properties_list:
- description: ''
  name: channels
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-list-channels-response-schema.json
slug: ivs-list-channels-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-channels-response-schema.json\",\n  \"title\": \"ListChannelsResponse\",\n  \"description\": \"ListChannelsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelList\"\n        },\n        {\n          \"description\": \"List of the matching channels.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If there are more channels than <code>maxResults</code>, use <code>nextToken</code> in the request to get the next set.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"channels\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-channels-response-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: ListChannelsResponse
---
