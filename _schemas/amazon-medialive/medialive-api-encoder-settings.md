---
description: Encoder Settings
layout: schema
name: EncoderSettings
properties_list:
- description: ''
  name: AudioDescriptions
  type: object
- description: ''
  name: AvailBlanking
  type: object
- description: ''
  name: AvailConfiguration
  type: object
- description: ''
  name: BlackoutSlate
  type: object
- description: ''
  name: CaptionDescriptions
  type: object
- description: ''
  name: FeatureActivations
  type: object
- description: ''
  name: GlobalConfiguration
  type: object
- description: ''
  name: MotionGraphicsConfiguration
  type: object
- description: ''
  name: NielsenConfiguration
  type: object
- description: ''
  name: OutputGroups
  type: object
- description: ''
  name: TimecodeConfig
  type: object
- description: ''
  name: VideoDescriptions
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-encoder-settings-schema.json
slug: medialive-api-encoder-settings
source_filename: medialive-api-encoder-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-encoder-settings-schema.json\",\n  \"title\": \"EncoderSettings\",\n  \"description\": \"Encoder Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAudioDescription\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioDescriptions\"\n          }\n        }\n      ]\n    },\n    \"AvailBlanking\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailBlanking\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"availBlanking\"\n          },\n          \"description\": \"Settings for ad avail blanking.\"\n        }\n      ]\n    },\n    \"AvailConfiguration\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/AvailConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"availConfiguration\"\n          },\n          \"description\": \"Event-wide configuration settings for ad avail insertion.\"\n        }\n      ]\n    },\n    \"BlackoutSlate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlackoutSlate\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"blackoutSlate\"\n          },\n          \"description\": \"Settings for blackout slate.\"\n        }\n      ]\n    },\n    \"CaptionDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfCaptionDescription\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captionDescriptions\"\n          },\n          \"description\": \"Settings for caption decriptions\"\n        }\n      ]\n    },\n    \"FeatureActivations\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/FeatureActivations\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"featureActivations\"\n          },\n          \"description\": \"Feature Activations\"\n        }\n      ]\n    },\n    \"GlobalConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlobalConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"globalConfiguration\"\n          },\n          \"description\": \"Configuration settings that apply to the event as a whole.\"\n        }\n      ]\n    },\n    \"MotionGraphicsConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MotionGraphicsConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"motionGraphicsConfiguration\"\n          },\n          \"description\": \"Settings for motion graphics.\"\n        }\n      ]\n    },\n    \"NielsenConfiguration\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/NielsenConfiguration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nielsenConfiguration\"\n          },\n          \"description\": \"Nielsen configuration settings.\"\n        }\n      ]\n    },\n    \"OutputGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOutputGroup\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputGroups\"\n          }\n        }\n      ]\n    },\n    \"TimecodeConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimecodeConfig\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timecodeConfig\"\n          },\n          \"description\": \"Contains settings used to acquire and adjust timecode information from inputs.\"\n        }\n      ]\n    },\n    \"VideoDescriptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfVideoDescription\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"videoDescriptions\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VideoDescriptions\",\n    \"AudioDescriptions\",\n    \"OutputGroups\",\n    \"TimecodeConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-encoder-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: EncoderSettings
---
