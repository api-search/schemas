---
description: ListRecordingConfigurationsRequest schema
layout: schema
name: ListRecordingConfigurationsRequest
properties_list:
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-list-recording-configurations-request-schema.json
slug: ivs-list-recording-configurations-request
source_filename: ivs-list-recording-configurations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-recording-configurations-request-schema.json\",\n  \"title\": \"ListRecordingConfigurationsRequest\",\n  \"description\": \"ListRecordingConfigurationsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxRecordingConfigurationResults\"\n        },\n        {\n          \"description\": \"Maximum number of recording configurations to return. Default: your service quota or 100, whichever is smaller. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The first recording configuration to retrieve. This is used for pagination;\
  \ see the <code>nextToken</code> response field.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-recording-configurations-request-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: ListRecordingConfigurationsRequest
---
