---
description: Settings for preset
layout: schema
name: PresetSettings
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
  name: VideoDescription
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-preset-settings-schema.json
slug: mediaconvert-api-preset-settings
source_filename: mediaconvert-api-preset-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-preset-settings-schema.json\",\n  \"title\": \"PresetSettings\",\n  \"description\": \"Settings for preset\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAudioDescription\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioDescriptions\"\n          },\n          \"description\": \"(AudioDescriptions) contains groups of audio encoding settings organized by audio codec. Include one instance of (AudioDescriptions) per output. (AudioDescriptions) can contain multiple groups of encoding settings.\"\n        }\n      ]\n    },\n    \"CaptionDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfCaptionDescriptionPreset\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"captionDescriptions\"\n          },\n          \"description\": \"This object holds groups of settings related to captions for one output. For each output that has captions, include one instance of CaptionDescriptions.\"\n        }\n      ]\n    },\n    \"ContainerSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"containerSettings\"\n          },\n          \"description\": \"Container specific settings.\"\n        }\n      ]\n    },\n    \"VideoDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoDescription\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoDescription\"\n          },\n          \"description\": \"VideoDescription contains a group of video encoding settings. The specific video settings depend on the video\
  \ codec that you choose for the property codec. Include one instance of VideoDescription per output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-preset-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: PresetSettings
---
