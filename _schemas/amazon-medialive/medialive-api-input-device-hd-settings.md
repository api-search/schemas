---
description: Settings that describe the active source from the input device, and the video characteristics of that source.
layout: schema
name: InputDeviceHdSettings
properties_list:
- description: ''
  name: ActiveInput
  type: object
- description: ''
  name: ConfiguredInput
  type: object
- description: ''
  name: DeviceState
  type: object
- description: ''
  name: Framerate
  type: object
- description: ''
  name: Height
  type: object
- description: ''
  name: MaxBitrate
  type: object
- description: ''
  name: ScanType
  type: object
- description: ''
  name: Width
  type: object
- description: ''
  name: LatencyMs
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-device-hd-settings-schema.json
slug: medialive-api-input-device-hd-settings
source_filename: medialive-api-input-device-hd-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-device-hd-settings-schema.json\",\n  \"title\": \"InputDeviceHdSettings\",\n  \"description\": \"Settings that describe the active source from the input device, and the video characteristics of that source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActiveInput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeviceActiveInput\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"activeInput\"\n          },\n          \"description\": \"If you specified Auto as the configured input, specifies which of the sources is currently active (SDI or HDMI).\"\n        }\n      ]\n    },\n    \"ConfiguredInput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeviceConfiguredInput\"\n       \
  \ },\n        {\n          \"xml\": {\n            \"name\": \"configuredInput\"\n          },\n          \"description\": \"The source at the input device that is currently active. You can specify this source.\"\n        }\n      ]\n    },\n    \"DeviceState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeviceState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deviceState\"\n          },\n          \"description\": \"The state of the input device.\"\n        }\n      ]\n    },\n    \"Framerate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"framerate\"\n          },\n          \"description\": \"The frame rate of the video source.\"\n        }\n      ]\n    },\n    \"Height\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"height\"\n          },\n          \"description\": \"The height of the video source, in pixels.\"\n        }\n      ]\n    },\n    \"MaxBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxBitrate\"\n          },\n          \"description\": \"The current maximum bitrate for ingesting this source, in bits per second. You can specify this maximum.\"\n        }\n      ]\n    },\n    \"ScanType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeviceScanType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scanType\"\n          },\n          \"description\": \"The scan type of the video source.\"\n        }\n      ]\n    },\n    \"Width\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"width\"\n          },\n          \"description\": \"The width of the video source, in pixels.\"\n        }\n      ]\n    },\n    \"LatencyMs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"latencyMs\"\n          },\n          \"description\": \"The Link device's buffer size (latency) in milliseconds (ms). You can specify this value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-device-hd-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputDeviceHdSettings
---
