---
description: GetRecordingConfigurationResponse schema
layout: schema
name: GetRecordingConfigurationResponse
properties_list:
- description: ''
  name: recordingConfiguration
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-get-recording-configuration-response-schema.json
slug: ivs-get-recording-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-recording-configuration-response-schema.json\",\n  \"title\": \"GetRecordingConfigurationResponse\",\n  \"description\": \"GetRecordingConfigurationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recordingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordingConfiguration\"\n        },\n        {\n          \"description\": \"<zonbook></zonbook><xhtml></xhtml>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-get-recording-configuration-response-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: GetRecordingConfigurationResponse
---
