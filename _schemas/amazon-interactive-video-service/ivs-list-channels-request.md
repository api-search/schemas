---
description: ListChannelsRequest schema
layout: schema
name: ListChannelsRequest
properties_list:
- description: ''
  name: filterByName
  type: object
- description: ''
  name: filterByRecordingConfigurationArn
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-list-channels-request-schema.json
slug: ivs-list-channels-request
source_filename: ivs-list-channels-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-channels-request-schema.json\",\n  \"title\": \"ListChannelsRequest\",\n  \"description\": \"ListChannelsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filterByName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelName\"\n        },\n        {\n          \"description\": \"Filters the channel list to match the specified name.\"\n        }\n      ]\n    },\n    \"filterByRecordingConfigurationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelRecordingConfigurationArn\"\n        },\n        {\n          \"description\": \"Filters the channel list to match the specified recording-configuration ARN.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/MaxChannelResults\"\n        },\n        {\n          \"description\": \"Maximum number of channels to return. Default: 100.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The first channel to retrieve. This is used for pagination; see the <code>nextToken</code> response field.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-channels-request-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: ListChannelsRequest
---
