---
description: CreateRecordingConfigurationRequest schema
layout: schema
name: CreateRecordingConfigurationRequest
properties_list:
- description: ''
  name: destinationConfiguration
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: recordingReconnectWindowSeconds
  type: object
- description: ''
  name: renditionConfiguration
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: thumbnailConfiguration
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-create-recording-configuration-request-schema.json
slug: ivs-create-recording-configuration-request
source_filename: ivs-create-recording-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-create-recording-configuration-request-schema.json\",\n  \"title\": \"CreateRecordingConfigurationRequest\",\n  \"description\": \"CreateRecordingConfigurationRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destinationConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationConfiguration\"\n        },\n        {\n          \"description\": \"A complex type that contains a destination configuration for where recorded video will be stored.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordingConfigurationName\"\n        },\n        {\n          \"description\": \"Recording-configuration name. The value does not need to be unique.\"\n   \
  \     }\n      ]\n    },\n    \"recordingReconnectWindowSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordingReconnectWindowSeconds\"\n        },\n        {\n          \"description\": \"If a broadcast disconnects and then reconnects within the specified interval, the multiple streams will be considered a single broadcast and merged together. Default: 0.\"\n        }\n      ]\n    },\n    \"renditionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RenditionConfiguration\"\n        },\n        {\n          \"description\": \"Object that describes which renditions should be recorded for a stream.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"Array of 1-50 maps, each of the form <code>string:string (key:value)</code>. See <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\\\
  \">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \\\"Tag naming limits and requirements\\\"; Amazon IVS has no service-specific constraints beyond what is documented there.\"\n        }\n      ]\n    },\n    \"thumbnailConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThumbnailConfiguration\"\n        },\n        {\n          \"description\": \"A complex type that allows you to enable/disable the recording of thumbnails for a live session and modify the interval at which thumbnails are generated for the live session.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"destinationConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-create-recording-configuration-request-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: CreateRecordingConfigurationRequest
---
