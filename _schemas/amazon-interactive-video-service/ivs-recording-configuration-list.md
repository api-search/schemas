---
description: RecordingConfigurationList schema
layout: schema
name: RecordingConfigurationList
properties_list: []
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-recording-configuration-list-schema.json
slug: ivs-recording-configuration-list
source_filename: ivs-recording-configuration-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-recording-configuration-list-schema.json\",\n  \"title\": \"RecordingConfigurationList\",\n  \"description\": \"RecordingConfigurationList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"arn\",\n      \"destinationConfiguration\",\n      \"state\"\n    ],\n    \"properties\": {\n      \"arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/RecordingConfigurationArn\"\n          },\n          {\n            \"description\": \"Recording-configuration ARN.\"\n          }\n        ]\n      },\n      \"destinationConfiguration\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DestinationConfiguration\"\n          },\n          {\n            \"description\"\
  : \"A complex type that contains information about where recorded video will be stored.\"\n          }\n        ]\n      },\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/RecordingConfigurationName\"\n          },\n          {\n            \"description\": \"Recording-configuration name. The value does not need to be unique.\"\n          }\n        ]\n      },\n      \"state\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/RecordingConfigurationState\"\n          },\n          {\n            \"description\": \"Indicates the current state of the recording configuration. When the state is <code>ACTIVE</code>, the configuration is ready for recording a channel stream.\"\n          }\n        ]\n      },\n      \"tags\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Tags\"\n          },\n          {\n            \"description\": \"Tags attached to the resource. Array\
  \ of 1-50 maps, each of the form <code>string:string (key:value)</code>. See <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\\\">Tagging Amazon Web Services Resources</a> for more information, including restrictions that apply to tags and \\\"Tag naming limits and requirements\\\"; Amazon IVS has no service-specific constraints beyond what is documented there.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Summary information about a RecordingConfiguration.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-recording-configuration-list-schema.json
tags:
- Live Streaming
- Media
- Video
- Real-Time
title: RecordingConfigurationList
---
