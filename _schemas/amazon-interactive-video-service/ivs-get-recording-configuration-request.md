---
description: GetRecordingConfigurationRequest schema
layout: schema
name: GetRecordingConfigurationRequest
properties_list:
- description: ''
  name: arn
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-get-recording-configuration-request-schema.json
slug: ivs-get-recording-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-recording-configuration-request-schema.json\",\n  \"title\": \"GetRecordingConfigurationRequest\",\n  \"description\": \"GetRecordingConfigurationRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordingConfigurationArn\"\n        },\n        {\n          \"description\": \"ARN of the recording configuration to be retrieved.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-recording-configuration-request-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: GetRecordingConfigurationRequest
---
