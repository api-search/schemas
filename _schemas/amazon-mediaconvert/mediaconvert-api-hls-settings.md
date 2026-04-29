---
description: Settings for HLS output groups
layout: schema
name: HlsSettings
properties_list:
- description: ''
  name: AudioGroupId
  type: object
- description: ''
  name: AudioOnlyContainer
  type: object
- description: ''
  name: AudioRenditionSets
  type: object
- description: ''
  name: AudioTrackType
  type: object
- description: ''
  name: DescriptiveVideoServiceFlag
  type: object
- description: ''
  name: IFrameOnlyManifest
  type: object
- description: ''
  name: SegmentModifier
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-settings-schema.json
slug: mediaconvert-api-hls-settings
source_filename: mediaconvert-api-hls-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-settings-schema.json\",\n  \"title\": \"HlsSettings\",\n  \"description\": \"Settings for HLS output groups\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioGroupId\"\n          },\n          \"description\": \"Specifies the group to which the audio rendition belongs.\"\n        }\n      ]\n    },\n    \"AudioOnlyContainer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsAudioOnlyContainer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioOnlyContainer\"\n          },\n          \"description\": \"Use this setting only in audio-only outputs.\
  \ Choose MPEG-2 Transport Stream (M2TS) to create a file in an MPEG2-TS container. Keep the default value Automatic (AUTOMATIC) to create an audio-only file in a raw container. Regardless of the value that you specify here, if this output has video, the service will place the output into an MPEG2-TS container.\"\n        }\n      ]\n    },\n    \"AudioRenditionSets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioRenditionSets\"\n          },\n          \"description\": \"List all the audio groups that are used with the video output stream. Input all the audio GROUP-IDs that are associated to the video, separate by ','.\"\n        }\n      ]\n    },\n    \"AudioTrackType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsAudioTrackType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioTrackType\"\n          },\n\
  \          \"description\": \"Four types of audio-only tracks are supported: Audio-Only Variant Stream The client can play back this audio-only stream instead of video in low-bandwidth scenarios. Represented as an EXT-X-STREAM-INF in the HLS manifest. Alternate Audio, Auto Select, Default Alternate rendition that the client should try to play back by default. Represented as an EXT-X-MEDIA in the HLS manifest with DEFAULT=YES, AUTOSELECT=YES Alternate Audio, Auto Select, Not Default Alternate rendition that the client may try to play back by default. Represented as an EXT-X-MEDIA in the HLS manifest with DEFAULT=NO, AUTOSELECT=YES Alternate Audio, not Auto Select Alternate rendition that the client will not try to play back by default. Represented as an EXT-X-MEDIA in the HLS manifest with DEFAULT=NO, AUTOSELECT=NO\"\n        }\n      ]\n    },\n    \"DescriptiveVideoServiceFlag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsDescriptiveVideoServiceFlag\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"descriptiveVideoServiceFlag\"\n          },\n          \"description\": \"Specify whether to flag this audio track as descriptive video service (DVS) in your HLS parent manifest. When you choose Flag (FLAG), MediaConvert includes the parameter CHARACTERISTICS=\\\"public.accessibility.describes-video\\\" in the EXT-X-MEDIA entry for this track. When you keep the default choice, Don't flag (DONT_FLAG), MediaConvert leaves this parameter out. The DVS flag can help with accessibility on Apple devices. For more information, see the Apple documentation.\"\n        }\n      ]\n    },\n    \"IFrameOnlyManifest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsIFrameOnlyManifest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"iFrameOnlyManifest\"\n          },\n          \"description\": \"Choose Include (INCLUDE) to have MediaConvert generate a child manifest that lists\
  \ only the I-frames for this rendition, in addition to your regular manifest for this rendition. You might use this manifest as part of a workflow that creates preview functions for your video. MediaConvert adds both the I-frame only child manifest and the regular child manifest to the parent manifest. When you don't need the I-frame only child manifest, keep the default value Exclude (EXCLUDE).\"\n        }\n      ]\n    },\n    \"SegmentModifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentModifier\"\n          },\n          \"description\": \"Use this setting to add an identifying string to the filename of each segment. The service adds this string between the name modifier and segment index number. You can use format identifiers in the string. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/using-variables-in-your-job-settings.html\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsSettings
---
