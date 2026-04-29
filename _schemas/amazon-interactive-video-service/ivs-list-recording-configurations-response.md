---
description: ListRecordingConfigurationsResponse schema
layout: schema
name: ListRecordingConfigurationsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: recordingConfigurations
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-list-recording-configurations-response-schema.json
slug: ivs-list-recording-configurations-response
source_filename: ivs-list-recording-configurations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-recording-configurations-response-schema.json\",\n  \"title\": \"ListRecordingConfigurationsResponse\",\n  \"description\": \"ListRecordingConfigurationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If there are more recording configurations than <code>maxResults</code>, use <code>nextToken</code> in the request to get the next set.\"\n        }\n      ]\n    },\n    \"recordingConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordingConfigurationList\"\n        },\n        {\n          \"description\": \"List of the matching recording configurations.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"recordingConfigurations\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-list-recording-configurations-response-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: ListRecordingConfigurationsResponse
---
