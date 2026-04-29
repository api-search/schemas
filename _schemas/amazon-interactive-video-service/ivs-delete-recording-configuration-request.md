---
description: DeleteRecordingConfigurationRequest schema
layout: schema
name: DeleteRecordingConfigurationRequest
properties_list:
- description: ''
  name: arn
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-delete-recording-configuration-request-schema.json
slug: ivs-delete-recording-configuration-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-delete-recording-configuration-request-schema.json\",\n  \"title\": \"DeleteRecordingConfigurationRequest\",\n  \"description\": \"DeleteRecordingConfigurationRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordingConfigurationArn\"\n        },\n        {\n          \"description\": \"ARN of the recording configuration to be deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-delete-recording-configuration-request-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: DeleteRecordingConfigurationRequest
---
