---
description: Each output in your job is a collection of settings that describes how you want MediaConvert to encode a single output file or stream. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/create-outputs.html.
layout: schema
name: Output
properties_list:
- description: ''
  name: AudioDescriptions
  type: object
- description: ''
  name: CaptionDescriptions
  type: object
- description: ''
  name: ContainerSettings
  type: object
- description: ''
  name: Extension
  type: object
- description: ''
  name: NameModifier
  type: object
- description: ''
  name: OutputSettings
  type: object
- description: ''
  name: Preset
  type: object
- description: ''
  name: VideoDescription
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-output-schema.json
slug: mediaconvert-api-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-schema.json\",\n  \"title\": \"Output\",\n  \"description\": \"Each output in your job is a collection of settings that describes how you want MediaConvert to encode a single output file or stream. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/create-outputs.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAudioDescription\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioDescriptions\"\n          },\n          \"description\": \"(AudioDescriptions) contains groups of audio encoding settings organized by audio codec. Include one instance of (AudioDescriptions) per output. (AudioDescriptions) can contain\
  \ multiple groups of encoding settings.\"\n        }\n      ]\n    },\n    \"CaptionDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfCaptionDescription\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captionDescriptions\"\n          },\n          \"description\": \"(CaptionDescriptions) contains groups of captions settings. For each output that has captions, include one instance of (CaptionDescriptions). (CaptionDescriptions) can contain multiple groups of captions settings.\"\n        }\n      ]\n    },\n    \"ContainerSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"containerSettings\"\n          },\n          \"description\": \"Container specific settings.\"\n        }\n      ]\n    },\n    \"Extension\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"extension\"\n          },\n          \"description\": \"Use Extension (Extension) to specify the file extension for outputs in File output groups. If you do not specify a value, the service will use default extensions by container type as follows * MPEG-2 transport stream, m2ts * Quicktime, mov * MXF container, mxf * MPEG-4 container, mp4 * WebM container, webm * No Container, the service will use codec extensions (e.g. AAC, H265, H265, AC3)\"\n        }\n      ]\n    },\n    \"NameModifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nameModifier\"\n          },\n          \"description\": \"Use Name modifier (NameModifier) to have the service add a string to the end of each output filename. You specify the base filename as part of your destination URI. When you create multiple outputs in the same\
  \ output group, Name modifier (NameModifier) is required. Name modifier also accepts format identifiers. For DASH ISO outputs, if you use the format identifiers $Number$ or $Time$ in one output, you must use them in the same way in all outputs of the output group.\"\n        }\n      ]\n    },\n    \"OutputSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputSettings\"\n          },\n          \"description\": \"Specific settings for this type of output.\"\n        }\n      ]\n    },\n    \"Preset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"preset\"\n          },\n          \"description\": \"Use Preset (Preset) to specify a preset for your transcoding settings. Provide the system or custom preset name. You can specify either Preset (Preset)\
  \ or Container settings (ContainerSettings), but not both.\"\n        }\n      ]\n    },\n    \"VideoDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoDescription\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoDescription\"\n          },\n          \"description\": \"VideoDescription contains a group of video encoding settings. The specific video settings depend on the video codec that you choose for the property codec. Include one instance of VideoDescription per output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Output
---
