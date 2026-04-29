---
description: Video codec settings, (CodecSettings) under (VideoDescription), contains the group of settings related to video encoding. The settings in this group vary depending on the value that you choose for Video codec (Codec). For each codec enum that you choose, define the corresponding settings object. The following lists the codec enum, settings object pairs. * AV1, Av1Settings * AVC_INTRA, AvcIntraSettings * FRAME_CAPTURE, FrameCaptureSettings * H_264, H264Settings * H_265, H265Settings * MPEG2, Mpeg2Settings * PRORES, ProresSettings * VC3, Vc3Settings * VP8, Vp8Settings * VP9, Vp9Settings * XAVC, XavcSettings
layout: schema
name: VideoCodecSettings
properties_list:
- description: ''
  name: Av1Settings
  type: object
- description: ''
  name: AvcIntraSettings
  type: object
- description: ''
  name: Codec
  type: object
- description: ''
  name: FrameCaptureSettings
  type: object
- description: ''
  name: H264Settings
  type: object
- description: ''
  name: H265Settings
  type: object
- description: ''
  name: Mpeg2Settings
  type: object
- description: ''
  name: ProresSettings
  type: object
- description: ''
  name: Vc3Settings
  type: object
- description: ''
  name: Vp8Settings
  type: object
- description: ''
  name: Vp9Settings
  type: object
- description: ''
  name: XavcSettings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-video-codec-settings-schema.json
slug: mediaconvert-api-video-codec-settings
source_filename: mediaconvert-api-video-codec-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-video-codec-settings-schema.json\",\n  \"title\": \"VideoCodecSettings\",\n  \"description\": \"Video codec settings, (CodecSettings) under (VideoDescription), contains the group of settings related to video encoding. The settings in this group vary depending on the value that you choose for Video codec (Codec). For each codec enum that you choose, define the corresponding settings object. The following lists the codec enum, settings object pairs. * AV1, Av1Settings * AVC_INTRA, AvcIntraSettings * FRAME_CAPTURE, FrameCaptureSettings * H_264, H264Settings * H_265, H265Settings * MPEG2, Mpeg2Settings * PRORES, ProresSettings * VC3, Vc3Settings * VP8, Vp8Settings * VP9, Vp9Settings * XAVC, XavcSettings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Av1Settings\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Av1Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"av1Settings\"\n          },\n          \"description\": \"Required when you set Codec, under VideoDescription>CodecSettings to the value AV1.\"\n        }\n      ]\n    },\n    \"AvcIntraSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvcIntraSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"avcIntraSettings\"\n          },\n          \"description\": \"Required when you choose AVC-Intra for your output video codec. For more information about the AVC-Intra settings, see the relevant specification. For detailed information about SD and HD in AVC-Intra, see https://ieeexplore.ieee.org/document/7290936. For information about 4K/2K in AVC-Intra, see https://pro-av.panasonic.net/en/avc-ultra/AVC-ULTRAoverview.pdf.\"\n        }\n      ]\n    },\n    \"Codec\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/VideoCodec\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codec\"\n          },\n          \"description\": \"Specifies the video codec. This must be equal to one of the enum values defined by the object VideoCodec.\"\n        }\n      ]\n    },\n    \"FrameCaptureSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrameCaptureSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"frameCaptureSettings\"\n          },\n          \"description\": \"Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value FRAME_CAPTURE.\"\n        }\n      ]\n    },\n    \"H264Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H264Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"h264Settings\"\n          },\n          \"description\": \"Required when you set (Codec)\
  \ under (VideoDescription)>(CodecSettings) to the value H_264.\"\n        }\n      ]\n    },\n    \"H265Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/H265Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"h265Settings\"\n          },\n          \"description\": \"Settings for H265 codec\"\n        }\n      ]\n    },\n    \"Mpeg2Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mpeg2Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mpeg2Settings\"\n          },\n          \"description\": \"Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value MPEG2.\"\n        }\n      ]\n    },\n    \"ProresSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProresSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"proresSettings\"\n          },\n          \"description\"\
  : \"Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value PRORES.\"\n        }\n      ]\n    },\n    \"Vc3Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vc3Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vc3Settings\"\n          },\n          \"description\": \"Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value VC3\"\n        }\n      ]\n    },\n    \"Vp8Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vp8Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vp8Settings\"\n          },\n          \"description\": \"Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value VP8.\"\n        }\n      ]\n    },\n    \"Vp9Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Vp9Settings\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"vp9Settings\"\n          },\n          \"description\": \"Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value VP9.\"\n        }\n      ]\n    },\n    \"XavcSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XavcSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"xavcSettings\"\n          },\n          \"description\": \"Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value XAVC.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-video-codec-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: VideoCodecSettings
---
