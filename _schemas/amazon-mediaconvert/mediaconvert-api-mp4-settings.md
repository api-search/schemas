---
description: These settings relate to your MP4 output container. You can create audio only outputs with this container. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/supported-codecs-containers-audio-only.html#output-codecs-and-containers-supported-for-audio-only.
layout: schema
name: Mp4Settings
properties_list:
- description: ''
  name: AudioDuration
  type: object
- description: ''
  name: CslgAtom
  type: object
- description: ''
  name: CttsVersion
  type: object
- description: ''
  name: FreeSpaceBox
  type: object
- description: ''
  name: MoovPlacement
  type: object
- description: ''
  name: Mp4MajorBrand
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-mp4-settings-schema.json
slug: mediaconvert-api-mp4-settings
source_filename: mediaconvert-api-mp4-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mp4-settings-schema.json\",\n  \"title\": \"Mp4Settings\",\n  \"description\": \"These settings relate to your MP4 output container. You can create audio only outputs with this container. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/supported-codecs-containers-audio-only.html#output-codecs-and-containers-supported-for-audio-only.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmfcAudioDuration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioDuration\"\n          },\n          \"description\": \"Specify this setting only when your output will be consumed by a downstream repackaging workflow that is sensitive to very small\
  \ duration differences between video and audio. For this situation, choose Match video duration (MATCH_VIDEO_DURATION). In all other cases, keep the default value, Default codec duration (DEFAULT_CODEC_DURATION). When you choose Match video duration, MediaConvert pads the output audio streams with silence or trims them to ensure that the total duration of each audio stream is at least as long as the total duration of the video stream. After padding or trimming, the audio stream duration is no more than one frame longer than the video stream. MediaConvert applies audio padding or trimming only to the end of the last segment of the output. For unsegmented outputs, MediaConvert adds padding only to the end of the file. When you keep the default value, any minor discrepancies between audio and video duration will depend on your output audio codec.\"\n        }\n      ]\n    },\n    \"CslgAtom\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mp4CslgAtom\"\n  \
  \      },\n        {\n          \"xml\": {\n            \"name\": \"cslgAtom\"\n          },\n          \"description\": \"When enabled, file composition times will start at zero, composition times in the 'ctts' (composition time to sample) box for B-frames will be negative, and a 'cslg' (composition shift least greatest) box will be included per 14496-1 amendment 1. This improves compatibility with Apple players and tools.\"\n        }\n      ]\n    },\n    \"CttsVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cttsVersion\"\n          },\n          \"description\": \"Ignore this setting unless compliance to the CTTS box version specification matters in your workflow. Specify a value of 1 to set your CTTS box version to 1 and make your output compliant with the specification. When you specify a value of 1, you must also set CSLG atom (cslgAtom) to the value\
  \ INCLUDE. Keep the default value 0 to set your CTTS box version to 0. This can provide backward compatibility for some players and packagers.\"\n        }\n      ]\n    },\n    \"FreeSpaceBox\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mp4FreeSpaceBox\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"freeSpaceBox\"\n          },\n          \"description\": \"Inserts a free-space box immediately after the moov box.\"\n        }\n      ]\n    },\n    \"MoovPlacement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mp4MoovPlacement\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"moovPlacement\"\n          },\n          \"description\": \"If set to PROGRESSIVE_DOWNLOAD, the MOOV atom is relocated to the beginning of the archive as required for progressive downloading. Otherwise it is placed normally at the end.\"\n        }\n      ]\n    },\n    \"Mp4MajorBrand\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mp4MajorBrand\"\n          },\n          \"description\": \"Overrides the \\\"Major Brand\\\" field in the output file. Usually not necessary to specify.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mp4-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Mp4Settings
---
