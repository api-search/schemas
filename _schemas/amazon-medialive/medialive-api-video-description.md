---
description: Video settings for this stream.
layout: schema
name: VideoDescription
properties_list:
- description: ''
  name: CodecSettings
  type: object
- description: ''
  name: Height
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RespondToAfd
  type: object
- description: ''
  name: ScalingBehavior
  type: object
- description: ''
  name: Sharpness
  type: object
- description: ''
  name: Width
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-video-description-schema.json
slug: medialive-api-video-description
source_filename: medialive-api-video-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-description-schema.json\",\n  \"title\": \"VideoDescription\",\n  \"description\": \"Video settings for this stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodecSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoCodecSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codecSettings\"\n          },\n          \"description\": \"Video codec settings.\"\n        }\n      ]\n    },\n    \"Height\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"height\"\n          },\n          \"description\": \"Output video height, in pixels. Must be an even number. For most codecs, you can leave this field\
  \ and width blank in order to use the height and width (resolution) from the source. Note, however, that leaving blank is not recommended. For the Frame Capture codec, height and width are required.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of this VideoDescription. Outputs will use this name to uniquely identify this Description.  Description names should be unique within this Live Event.\"\n        }\n      ]\n    },\n    \"RespondToAfd\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoDescriptionRespondToAfd\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"respondToAfd\"\n          },\n          \"description\": \"Indicates how MediaLive will respond to the AFD values that might be in the input video. If you\
  \ do not know what AFD signaling is, or if your downstream system has not given you guidance, choose PASSTHROUGH.\\nRESPOND: MediaLive clips the input video using a formula that uses the AFD values (configured in afdSignaling ), the input display aspect ratio, and the output display aspect ratio. MediaLive also includes the AFD values in the output, unless the codec for this encode is FRAME_CAPTURE.\\nPASSTHROUGH: MediaLive ignores the AFD values and does not clip the video. But MediaLive does include the values in the output.\\nNONE: MediaLive does not clip the input video and does not include the AFD values in the output\"\n        }\n      ]\n    },\n    \"ScalingBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoDescriptionScalingBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scalingBehavior\"\n          },\n          \"description\": \"STRETCH_TO_OUTPUT configures the output position to stretch the video\
  \ to the specified output resolution (height and width). This option will override any position value. DEFAULT may insert black boxes (pillar boxes or letter boxes) around the video to provide the specified output resolution.\"\n        }\n      ]\n    },\n    \"Sharpness\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max100\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sharpness\"\n          },\n          \"description\": \"Changes the strength of the anti-alias filter used for scaling. 0 is the softest setting, 100 is the sharpest. A setting of 50 is recommended for most content.\"\n        }\n      ]\n    },\n    \"Width\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"width\"\n          },\n          \"description\": \"Output video width, in pixels. Must be an even number. For most codecs, you can leave\
  \ this field and height blank in order to use the height and width (resolution) from the source. Note, however, that leaving blank is not recommended. For the Frame Capture codec, height and width are required.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-description-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: VideoDescription
---
