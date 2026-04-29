---
description: JobSettings contains all the transcode settings for a job.
layout: schema
name: JobSettings
properties_list:
- description: ''
  name: AdAvailOffset
  type: object
- description: ''
  name: AvailBlanking
  type: object
- description: ''
  name: Esam
  type: object
- description: ''
  name: ExtendedDataServices
  type: object
- description: ''
  name: Inputs
  type: object
- description: ''
  name: KantarWatermark
  type: object
- description: ''
  name: MotionImageInserter
  type: object
- description: ''
  name: NielsenConfiguration
  type: object
- description: ''
  name: NielsenNonLinearWatermark
  type: object
- description: ''
  name: OutputGroups
  type: object
- description: ''
  name: TimecodeConfig
  type: object
- description: ''
  name: TimedMetadataInsertion
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-job-settings-schema.json
slug: mediaconvert-api-job-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-job-settings-schema.json\",\n  \"title\": \"JobSettings\",\n  \"description\": \"JobSettings contains all the transcode settings for a job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdAvailOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative1000Max1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adAvailOffset\"\n          },\n          \"description\": \"When specified, this offset (in milliseconds) is added to the input Ad Avail PTS time.\"\n        }\n      ]\n    },\n    \"AvailBlanking\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailBlanking\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"availBlanking\"\n          },\n  \
  \        \"description\": \"Settings for ad avail blanking. Video can be blanked or overlaid with an image, and audio muted during SCTE-35 triggered ad avails.\"\n        }\n      ]\n    },\n    \"Esam\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EsamSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"esam\"\n          },\n          \"description\": \"Settings for Event Signaling And Messaging (ESAM). If you don't do ad insertion, you can ignore these settings.\"\n        }\n      ]\n    },\n    \"ExtendedDataServices\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExtendedDataServices\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"extendedDataServices\"\n          },\n          \"description\": \"If your source content has EIA-608 Line 21 Data Services, enable this feature to specify what MediaConvert does with the Extended Data Services (XDS) packets. You can choose\
  \ to pass through XDS packets, or remove them from the output. For more information about XDS, see EIA-608 Line Data Services, section 9.5.1.5 05h Content Advisory.\"\n        }\n      ]\n    },\n    \"Inputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInput\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputs\"\n          },\n          \"description\": \"Use Inputs (inputs) to define source file used in the transcode job. There can be multiple inputs add in a job. These inputs will be concantenated together to create the output.\"\n        }\n      ]\n    },\n    \"KantarWatermark\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KantarWatermarkSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kantarWatermark\"\n          },\n          \"description\": \"Use these settings only when you use Kantar watermarking. Specify the values that MediaConvert uses to\
  \ generate and place Kantar watermarks in your output audio. These settings apply to every output in your job. In addition to specifying these values, you also need to store your Kantar credentials in AWS Secrets Manager. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/kantar-watermarking.html.\"\n        }\n      ]\n    },\n    \"MotionImageInserter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MotionImageInserter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"motionImageInserter\"\n          },\n          \"description\": \"Overlay motion graphics on top of your video. The motion graphics that you specify here appear on all outputs in all output groups. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/motion-graphic-overlay.html.\"\n        }\n      ]\n    },\n    \"NielsenConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NielsenConfiguration\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"nielsenConfiguration\"\n          },\n          \"description\": \"Settings for your Nielsen configuration. If you don't do Nielsen measurement and analytics, ignore these settings. When you enable Nielsen configuration (nielsenConfiguration), MediaConvert enables PCM to ID3 tagging for all outputs in the job. To enable Nielsen configuration programmatically, include an instance of nielsenConfiguration in your JSON job specification. Even if you don't include any children of nielsenConfiguration, you still enable the setting.\"\n        }\n      ]\n    },\n    \"NielsenNonLinearWatermark\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NielsenNonLinearWatermarkSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nielsenNonLinearWatermark\"\n          },\n          \"description\": \"Ignore these settings unless you are using Nielsen non-linear watermarking.\
  \ Specify the values that MediaConvert uses to generate and place Nielsen watermarks in your output audio. In addition to specifying these values, you also need to set up your cloud TIC server. These settings apply to every output in your job. The MediaConvert implementation is currently with the following Nielsen versions: Nielsen Watermark SDK Version 5.2.1 Nielsen NLM Watermark Engine Version 1.2.7 Nielsen Watermark Authenticator [SID_TIC] Version [5.0.0]\"\n        }\n      ]\n    },\n    \"OutputGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOutputGroup\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputGroups\"\n          },\n          \"description\": \"(OutputGroups) contains one group of settings for each set of outputs that share a common package type. All unpackaged files (MPEG-4, MPEG-2 TS, Quicktime, MXF, and no container) are grouped in a single output group as well. Required in (OutputGroups) is a\
  \ group of settings that apply to the whole group. This required object depends on the value you set for (Type) under (OutputGroups)>(OutputGroupSettings). Type, settings object pairs are as follows. * FILE_GROUP_SETTINGS, FileGroupSettings * HLS_GROUP_SETTINGS, HlsGroupSettings * DASH_ISO_GROUP_SETTINGS, DashIsoGroupSettings * MS_SMOOTH_GROUP_SETTINGS, MsSmoothGroupSettings * CMAF_GROUP_SETTINGS, CmafGroupSettings\"\n        }\n      ]\n    },\n    \"TimecodeConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimecodeConfig\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timecodeConfig\"\n          },\n          \"description\": \"These settings control how the service handles timecodes throughout the job. These settings don't affect input clipping.\"\n        }\n      ]\n    },\n    \"TimedMetadataInsertion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimedMetadataInsertion\"\n        },\n \
  \       {\n          \"xml\": {\n            \"name\": \"timedMetadataInsertion\"\n          },\n          \"description\": \"Insert user-defined custom ID3 metadata (id3) at timecodes (timecode) that you specify. In each output that you want to include this metadata, you must set ID3 metadata (timedMetadata) to Passthrough (PASSTHROUGH).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-job-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: JobSettings
---
