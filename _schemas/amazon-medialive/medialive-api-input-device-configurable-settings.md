---
description: Configurable settings for the input device.
layout: schema
name: InputDeviceConfigurableSettings
properties_list:
- description: ''
  name: ConfiguredInput
  type: object
- description: ''
  name: MaxBitrate
  type: object
- description: ''
  name: LatencyMs
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-device-configurable-settings-schema.json
slug: medialive-api-input-device-configurable-settings
source_filename: medialive-api-input-device-configurable-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-device-configurable-settings-schema.json\",\n  \"title\": \"InputDeviceConfigurableSettings\",\n  \"description\": \"Configurable settings for the input device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfiguredInput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeviceConfiguredInput\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"configuredInput\"\n          },\n          \"description\": \"The input source that you want to use. If the device has a source connected to only one of its input ports, or if you don't care which source the device sends, specify Auto. If the device has sources connected to both its input ports, and you want to use a specific source, specify the source.\"\n        }\n      ]\n\
  \    },\n    \"MaxBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxBitrate\"\n          },\n          \"description\": \"The maximum bitrate in bits per second. Set a value here to throttle the bitrate of the source video.\"\n        }\n      ]\n    },\n    \"LatencyMs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"latencyMs\"\n          },\n          \"description\": \"The Link device's buffer size (latency) in milliseconds (ms).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-device-configurable-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: InputDeviceConfigurableSettings
---
