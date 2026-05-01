---
description: These settings relate to the fragmented MP4 container for the segments in your CMAF outputs.
layout: schema
name: CmfcSettings
properties_list:
- description: ''
  name: AudioDuration
  type: object
- description: ''
  name: AudioGroupId
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
  name: KlvMetadata
  type: object
- description: ''
  name: ManifestMetadataSignaling
  type: object
- description: ''
  name: Scte35Esam
  type: object
- description: ''
  name: Scte35Source
  type: object
- description: ''
  name: TimedMetadata
  type: object
- description: ''
  name: TimedMetadataBoxVersion
  type: object
- description: ''
  name: TimedMetadataSchemeIdUri
  type: object
- description: ''
  name: TimedMetadataValue
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-cmfc-settings-schema.json
slug: mediaconvert-api-cmfc-settings
source_filename: mediaconvert-api-cmfc-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmfc-settings-schema.json\",\n  \"title\": \"CmfcSettings\",\n  \"description\": \"These settings relate to the fragmented MP4 container for the segments in your CMAF outputs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmfcAudioDuration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioDuration\"\n          },\n          \"description\": \"Specify this setting only when your output will be consumed by a downstream repackaging workflow that is sensitive to very small duration differences between video and audio. For this situation, choose Match video duration (MATCH_VIDEO_DURATION). In all other cases, keep the default value, Default codec duration (DEFAULT_CODEC_DURATION).\
  \ When you choose Match video duration, MediaConvert pads the output audio streams with silence or trims them to ensure that the total duration of each audio stream is at least as long as the total duration of the video stream. After padding or trimming, the audio stream duration is no more than one frame longer than the video stream. MediaConvert applies audio padding or trimming only to the end of the last segment of the output. For unsegmented outputs, MediaConvert adds padding only to the end of the file. When you keep the default value, any minor discrepancies between audio and video duration will depend on your output audio codec.\"\n        }\n      ]\n    },\n    \"AudioGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioGroupId\"\n          },\n          \"description\": \"Specify the audio rendition group for this audio rendition. Specify up to one value for\
  \ each audio output in your output group. This value appears in your HLS parent manifest in the EXT-X-MEDIA tag of TYPE=AUDIO, as the value for the GROUP-ID attribute. For example, if you specify \\\"audio_aac_1\\\" for Audio group ID, it appears in your manifest like this: #EXT-X-MEDIA:TYPE=AUDIO,GROUP-ID=\\\"audio_aac_1\\\". Related setting: To associate the rendition group that this audio track belongs to with a video rendition, include the same value that you provide here for that video output's setting Audio rendition sets (audioRenditionSets).\"\n        }\n      ]\n    },\n    \"AudioRenditionSets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioRenditionSets\"\n          },\n          \"description\": \"List the audio rendition groups that you want included with this video rendition. Use a comma-separated list. For example, say you want to include the audio rendition\
  \ groups that have the audio group IDs \\\"audio_aac_1\\\" and \\\"audio_dolby\\\". Then you would specify this value: \\\"audio_aac_1,audio_dolby\\\". Related setting: The rendition groups that you include in your comma-separated list should all match values that you specify in the setting Audio group ID (AudioGroupId) for audio renditions in the same output group as this video rendition. Default behavior: If you don't specify anything here and for Audio group ID, MediaConvert puts each audio variant in its own audio rendition group and associates it with every video variant. Each value in your list appears in your HLS parent manifest in the EXT-X-STREAM-INF tag as the value for the AUDIO attribute. To continue the previous example, say that the file name for the child manifest for your video rendition is \\\"amazing_video_1.m3u8\\\". Then, in your parent manifest, each value will appear on separate lines, like this: #EXT-X-STREAM-INF:AUDIO=\\\"audio_aac_1\\\"... amazing_video_1.m3u8\
  \ #EXT-X-STREAM-INF:AUDIO=\\\"audio_dolby\\\"... amazing_video_1.m3u8\"\n        }\n      ]\n    },\n    \"AudioTrackType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmfcAudioTrackType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioTrackType\"\n          },\n          \"description\": \"Use this setting to control the values that MediaConvert puts in your HLS parent playlist to control how the client player selects which audio track to play. The other options for this setting determine the values that MediaConvert writes for the DEFAULT and AUTOSELECT attributes of the EXT-X-MEDIA entry for the audio variant. For more information about these attributes, see the Apple documentation article https://developer.apple.com/documentation/http_live_streaming/example_playlists_for_http_live_streaming/adding_alternate_media_to_a_playlist. Choose Alternate audio, auto select, default (ALTERNATE_AUDIO_AUTO_SELECT_DEFAULT) to set DEFAULT=YES\
  \ and AUTOSELECT=YES. Choose this value for only one variant in your output group. Choose Alternate audio, auto select, not default (ALTERNATE_AUDIO_AUTO_SELECT) to set DEFAULT=NO and AUTOSELECT=YES. Choose Alternate Audio, Not Auto Select to set DEFAULT=NO and AUTOSELECT=NO. When you don't specify a value for this setting, MediaConvert defaults to Alternate audio, auto select, default. When there is more than one variant in your output group, you must explicitly choose a value for this setting.\"\n        }\n      ]\n    },\n    \"DescriptiveVideoServiceFlag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmfcDescriptiveVideoServiceFlag\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"descriptiveVideoServiceFlag\"\n          },\n          \"description\": \"Specify whether to flag this audio track as descriptive video service (DVS) in your HLS parent manifest. When you choose Flag (FLAG), MediaConvert includes the parameter CHARACTERISTICS=\\\
  \"public.accessibility.describes-video\\\" in the EXT-X-MEDIA entry for this track. When you keep the default choice, Don't flag (DONT_FLAG), MediaConvert leaves this parameter out. The DVS flag can help with accessibility on Apple devices. For more information, see the Apple documentation.\"\n        }\n      ]\n    },\n    \"IFrameOnlyManifest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmfcIFrameOnlyManifest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"iFrameOnlyManifest\"\n          },\n          \"description\": \"Choose Include (INCLUDE) to have MediaConvert generate an HLS child manifest that lists only the I-frames for this rendition, in addition to your regular manifest for this rendition. You might use this manifest as part of a workflow that creates preview functions for your video. MediaConvert adds both the I-frame only child manifest and the regular child manifest to the parent manifest. When you don't need the\
  \ I-frame only child manifest, keep the default value Exclude (EXCLUDE).\"\n        }\n      ]\n    },\n    \"KlvMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmfcKlvMetadata\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"klvMetadata\"\n          },\n          \"description\": \"To include key-length-value metadata in this output: Set KLV metadata insertion to Passthrough. MediaConvert reads KLV metadata present in your input and writes each instance to a separate event message box in the output, according to MISB ST1910.1. To exclude this KLV metadata: Set KLV metadata insertion to None or leave blank.\"\n        }\n      ]\n    },\n    \"ManifestMetadataSignaling\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmfcManifestMetadataSignaling\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestMetadataSignaling\"\n          },\n          \"description\": \"To add\
  \ an InbandEventStream element in your output MPD manifest for each type of event message, set Manifest metadata signaling to Enabled. For ID3 event messages, the InbandEventStream element schemeIdUri will be same value that you specify for ID3 metadata scheme ID URI. For SCTE35 event messages, the InbandEventStream element schemeIdUri will be \\\"urn:scte:scte35:2013:bin\\\". To leave these elements out of your output MPD manifest, set Manifest metadata signaling to Disabled. To enable Manifest metadata signaling, you must also set SCTE-35 source to Passthrough, ESAM SCTE-35 to insert, or ID3 metadata (TimedMetadata) to Passthrough.\"\n        }\n      ]\n    },\n    \"Scte35Esam\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmfcScte35Esam\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35Esam\"\n          },\n          \"description\": \"Use this setting only when you specify SCTE-35 markers from ESAM. Choose INSERT to put\
  \ SCTE-35 markers in this output at the insertion points that you specify in an ESAM XML document. Provide the document in the setting SCC XML (sccXml).\"\n        }\n      ]\n    },\n    \"Scte35Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmfcScte35Source\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35Source\"\n          },\n          \"description\": \"Ignore this setting unless you have SCTE-35 markers in your input video file. Choose Passthrough (PASSTHROUGH) if you want SCTE-35 markers that appear in your input to also appear in this output. Choose None (NONE) if you don't want those SCTE-35 markers in this output.\"\n        }\n      ]\n    },\n    \"TimedMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmfcTimedMetadata\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadata\"\n          },\n          \"description\": \"To include ID3 metadata\
  \ in this output: Set ID3 metadata (timedMetadata) to Passthrough (PASSTHROUGH). Specify this ID3 metadata in Custom ID3 metadata inserter (timedMetadataInsertion). MediaConvert writes each instance of ID3 metadata in a separate Event Message (eMSG) box. To exclude this ID3 metadata: Set ID3 metadata to None (NONE) or leave blank.\"\n        }\n      ]\n    },\n    \"TimedMetadataBoxVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmfcTimedMetadataBoxVersion\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataBoxVersion\"\n          },\n          \"description\": \"Specify the event message box (eMSG) version for ID3 timed metadata in your output.\\nFor more information, see ISO/IEC 23009-1:2022 section 5.10.3.3.3 Syntax.\\nLeave blank to use the default value Version 0.\\nWhen you specify Version 1, you must also set ID3 metadata (timedMetadata) to Passthrough.\"\n        }\n      ]\n    },\n    \"TimedMetadataSchemeIdUri\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMax1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataSchemeIdUri\"\n          },\n          \"description\": \"Specify the event message box (eMSG) scheme ID URI (scheme_id_uri) for ID3 timed metadata in your output. For more information, see ISO/IEC 23009-1:2022 section 5.10.3.3.4 Semantics. Leave blank to use the default value: https://aomedia.org/emsg/ID3 When you specify a value for ID3 metadata scheme ID URI, you must also set ID3 metadata (timedMetadata) to Passthrough.\"\n        }\n      ]\n    },\n    \"TimedMetadataValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMax1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataValue\"\n          },\n          \"description\": \"Specify the event message box (eMSG) value for ID3 timed metadata in your output. For more information,\
  \ see ISO/IEC 23009-1:2022 section 5.10.3.3.4 Semantics. When you specify a value for ID3 Metadata Value, you must also set ID3 metadata (timedMetadata) to Passthrough.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmfc-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CmfcSettings
---
