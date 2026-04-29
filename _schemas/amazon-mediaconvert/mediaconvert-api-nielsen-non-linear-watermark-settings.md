---
description: 'Ignore these settings unless you are using Nielsen non-linear watermarking. Specify the values that MediaConvert uses to generate and place Nielsen watermarks in your output audio. In addition to specifying these values, you also need to set up your cloud TIC server. These settings apply to every output in your job. The MediaConvert implementation is currently with the following Nielsen versions: Nielsen Watermark SDK Version 5.2.1 Nielsen NLM Watermark Engine Version 1.2.7 Nielsen Watermark Authenticator [SID_TIC] Version [5.0.0]'
layout: schema
name: NielsenNonLinearWatermarkSettings
properties_list:
- description: ''
  name: ActiveWatermarkProcess
  type: object
- description: ''
  name: AdiFilename
  type: object
- description: ''
  name: AssetId
  type: object
- description: ''
  name: AssetName
  type: object
- description: ''
  name: CbetSourceId
  type: object
- description: ''
  name: EpisodeId
  type: object
- description: ''
  name: MetadataDestination
  type: object
- description: ''
  name: SourceId
  type: object
- description: ''
  name: SourceWatermarkStatus
  type: object
- description: ''
  name: TicServerUrl
  type: object
- description: ''
  name: UniqueTicPerAudioTrack
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-nielsen-non-linear-watermark-settings-schema.json
slug: mediaconvert-api-nielsen-non-linear-watermark-settings
source_filename: mediaconvert-api-nielsen-non-linear-watermark-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-nielsen-non-linear-watermark-settings-schema.json\",\n  \"title\": \"NielsenNonLinearWatermarkSettings\",\n  \"description\": \"Ignore these settings unless you are using Nielsen non-linear watermarking. Specify the values that MediaConvert uses to generate and place Nielsen watermarks in your output audio. In addition to specifying these values, you also need to set up your cloud TIC server. These settings apply to every output in your job. The MediaConvert implementation is currently with the following Nielsen versions: Nielsen Watermark SDK Version 5.2.1 Nielsen NLM Watermark Engine Version 1.2.7 Nielsen Watermark Authenticator [SID_TIC] Version [5.0.0]\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActiveWatermarkProcess\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/NielsenActiveWatermarkProcessType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"activeWatermarkProcess\"\n          },\n          \"description\": \"Choose the type of Nielsen watermarks that you want in your outputs. When you choose NAES 2 and NW (NAES2_AND_NW), you must provide a value for the setting SID (sourceId). When you choose CBET (CBET), you must provide a value for the setting CSID (cbetSourceId). When you choose NAES 2, NW, and CBET (NAES2_AND_NW_AND_CBET), you must provide values for both of these settings.\"\n        }\n      ]\n    },\n    \"AdiFilename\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternS3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adiFilename\"\n          },\n          \"description\": \"Optional. Use this setting when you want the service to include an ADI file in the Nielsen metadata .zip file. To provide an ADI file, store\
  \ it in Amazon S3 and provide a URL to it here. The URL should be in the following format: S3://bucket/path/ADI-file. For more information about the metadata .zip file, see the setting Metadata destination (metadataDestination).\"\n        }\n      ]\n    },\n    \"AssetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max20\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"assetId\"\n          },\n          \"description\": \"Use the asset ID that you provide to Nielsen to uniquely identify this asset. Required for all Nielsen non-linear watermarking.\"\n        }\n      ]\n    },\n    \"AssetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max50\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"assetName\"\n          },\n          \"description\": \"Use the asset name that you provide to Nielsen for this asset. Required for all Nielsen non-linear watermarking.\"\
  \n        }\n      ]\n    },\n    \"CbetSourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPattern0xAFaF0908190908\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cbetSourceId\"\n          },\n          \"description\": \"Use the CSID that Nielsen provides to you. This CBET source ID should be unique to your Nielsen account but common to all of your output assets that have CBET watermarking. Required when you choose a value for the setting Watermark types (ActiveWatermarkProcess) that includes CBET.\"\n        }\n      ]\n    },\n    \"EpisodeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max20\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"episodeId\"\n          },\n          \"description\": \"Optional. If this asset uses an episode ID with Nielsen, provide it here.\"\n        }\n      ]\n    },\n    \"MetadataDestination\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternS3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"metadataDestination\"\n          },\n          \"description\": \"Specify the Amazon S3 location where you want MediaConvert to save your Nielsen non-linear metadata .zip file. This Amazon S3 bucket must be in the same Region as the one where you do your MediaConvert transcoding. If you want to include an ADI file in this .zip file, use the setting ADI file (adiFilename) to specify it. MediaConvert delivers the Nielsen metadata .zip files only to your metadata destination Amazon S3 bucket. It doesn't deliver the .zip files to Nielsen. You are responsible for delivering the metadata .zip files to Nielsen.\"\n        }\n      ]\n    },\n    \"SourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65534\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceId\"\n      \
  \    },\n          \"description\": \"Use the SID that Nielsen provides to you. This source ID should be unique to your Nielsen account but common to all of your output assets. Required for all Nielsen non-linear watermarking. This ID should be unique to your Nielsen account but common to all of your output assets. Required for all Nielsen non-linear watermarking.\"\n        }\n      ]\n    },\n    \"SourceWatermarkStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NielsenSourceWatermarkStatusType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceWatermarkStatus\"\n          },\n          \"description\": \"Required. Specify whether your source content already contains Nielsen non-linear watermarks. When you set this value to Watermarked (WATERMARKED), the service fails the job. Nielsen requires that you add non-linear watermarking to only clean content that doesn't already have non-linear Nielsen watermarks.\"\n        }\n\
  \      ]\n    },\n    \"TicServerUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternHttps\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ticServerUrl\"\n          },\n          \"description\": \"Specify the endpoint for the TIC server that you have deployed and configured in the AWS Cloud. Required for all Nielsen non-linear watermarking. MediaConvert can't connect directly to a TIC server. Instead, you must use API Gateway to provide a RESTful interface between MediaConvert and a TIC server that you deploy in your AWS account. For more information on deploying a TIC server in your AWS account and the required API Gateway, contact Nielsen support.\"\n        }\n      ]\n    },\n    \"UniqueTicPerAudioTrack\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NielsenUniqueTicPerAudioTrackType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"uniqueTicPerAudioTrack\"\
  \n          },\n          \"description\": \"To create assets that have the same TIC values in each audio track, keep the default value Share TICs (SAME_TICS_PER_TRACK). To create assets that have unique TIC values for each audio track, choose Use unique TICs (RESERVE_UNIQUE_TICS_PER_TRACK).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-nielsen-non-linear-watermark-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: NielsenNonLinearWatermarkSettings
---
