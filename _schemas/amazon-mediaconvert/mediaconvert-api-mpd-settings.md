---
description: These settings relate to the fragmented MP4 container for the segments in your DASH outputs.
layout: schema
name: MpdSettings
properties_list:
- description: ''
  name: AccessibilityCaptionHints
  type: object
- description: ''
  name: AudioDuration
  type: object
- description: ''
  name: CaptionContainerType
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
schema_file: json-schema/mediaconvert-api-mpd-settings-schema.json
slug: mediaconvert-api-mpd-settings
source_filename: mediaconvert-api-mpd-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mpd-settings-schema.json\",\n  \"title\": \"MpdSettings\",\n  \"description\": \"These settings relate to the fragmented MP4 container for the segments in your DASH outputs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessibilityCaptionHints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MpdAccessibilityCaptionHints\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accessibilityCaptionHints\"\n          },\n          \"description\": \"Optional. Choose Include (INCLUDE) to have MediaConvert mark up your DASH manifest with <Accessibility> elements for embedded 608 captions. This markup isn't generally required, but some video players require it to discover and play embedded 608 captions. Keep the default value, Exclude\
  \ (EXCLUDE), to leave these elements out. When you enable this setting, this is the markup that MediaConvert includes in your manifest: <Accessibility schemeIdUri=\\\"urn:scte:dash:cc:cea-608:2015\\\" value=\\\"CC1=eng\\\"/>\"\n        }\n      ]\n    },\n    \"AudioDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MpdAudioDuration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioDuration\"\n          },\n          \"description\": \"Specify this setting only when your output will be consumed by a downstream repackaging workflow that is sensitive to very small duration differences between video and audio. For this situation, choose Match video duration (MATCH_VIDEO_DURATION). In all other cases, keep the default value, Default codec duration (DEFAULT_CODEC_DURATION). When you choose Match video duration, MediaConvert pads the output audio streams with silence or trims them to ensure that the total duration of each audio\
  \ stream is at least as long as the total duration of the video stream. After padding or trimming, the audio stream duration is no more than one frame longer than the video stream. MediaConvert applies audio padding or trimming only to the end of the last segment of the output. For unsegmented outputs, MediaConvert adds padding only to the end of the file. When you keep the default value, any minor discrepancies between audio and video duration will depend on your output audio codec.\"\n        }\n      ]\n    },\n    \"CaptionContainerType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MpdCaptionContainerType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captionContainerType\"\n          },\n          \"description\": \"Use this setting only in DASH output groups that include sidecar TTML or IMSC captions. You specify sidecar captions in a separate output from your audio and video. Choose Raw (RAW) for captions in a single XML\
  \ file in a raw container. Choose Fragmented MPEG-4 (FRAGMENTED_MP4) for captions in XML format contained within fragmented MP4 files. This set of fragmented MP4 files is separate from your video and audio fragmented MP4 files.\"\n        }\n      ]\n    },\n    \"KlvMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MpdKlvMetadata\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"klvMetadata\"\n          },\n          \"description\": \"To include key-length-value metadata in this output: Set KLV metadata insertion to Passthrough. MediaConvert reads KLV metadata present in your input and writes each instance to a separate event message box in the output, according to MISB ST1910.1. To exclude this KLV metadata: Set KLV metadata insertion to None or leave blank.\"\n        }\n      ]\n    },\n    \"ManifestMetadataSignaling\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MpdManifestMetadataSignaling\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestMetadataSignaling\"\n          },\n          \"description\": \"To add an InbandEventStream element in your output MPD manifest for each type of event message, set Manifest metadata signaling to Enabled. For ID3 event messages, the InbandEventStream element schemeIdUri will be same value that you specify for ID3 metadata scheme ID URI. For SCTE35 event messages, the InbandEventStream element schemeIdUri will be \\\"urn:scte:scte35:2013:bin\\\". To leave these elements out of your output MPD manifest, set Manifest metadata signaling to Disabled. To enable Manifest metadata signaling, you must also set SCTE-35 source to Passthrough, ESAM SCTE-35 to insert, or ID3 metadata (TimedMetadata) to Passthrough.\"\n        }\n      ]\n    },\n    \"Scte35Esam\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MpdScte35Esam\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"scte35Esam\"\n          },\n          \"description\": \"Use this setting only when you specify SCTE-35 markers from ESAM. Choose INSERT to put SCTE-35 markers in this output at the insertion points that you specify in an ESAM XML document. Provide the document in the setting SCC XML (sccXml).\"\n        }\n      ]\n    },\n    \"Scte35Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MpdScte35Source\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35Source\"\n          },\n          \"description\": \"Ignore this setting unless you have SCTE-35 markers in your input video file. Choose Passthrough (PASSTHROUGH) if you want SCTE-35 markers that appear in your input to also appear in this output. Choose None (NONE) if you don't want those SCTE-35 markers in this output.\"\n        }\n      ]\n    },\n    \"TimedMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MpdTimedMetadata\"\n \
  \       },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadata\"\n          },\n          \"description\": \"To include ID3 metadata in this output: Set ID3 metadata (timedMetadata) to Passthrough (PASSTHROUGH). Specify this ID3 metadata in Custom ID3 metadata inserter (timedMetadataInsertion). MediaConvert writes each instance of ID3 metadata in a separate Event Message (eMSG) box. To exclude this ID3 metadata: Set ID3 metadata to None (NONE) or leave blank.\"\n        }\n      ]\n    },\n    \"TimedMetadataBoxVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MpdTimedMetadataBoxVersion\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataBoxVersion\"\n          },\n          \"description\": \"Specify the event message box (eMSG) version for ID3 timed metadata in your output.\\nFor more information, see ISO/IEC 23009-1:2022 section 5.10.3.3.3 Syntax.\\nLeave blank to use the default value Version\
  \ 0.\\nWhen you specify Version 1, you must also set ID3 metadata (timedMetadata) to Passthrough.\"\n        }\n      ]\n    },\n    \"TimedMetadataSchemeIdUri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMax1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataSchemeIdUri\"\n          },\n          \"description\": \"Specify the event message box (eMSG) scheme ID URI (scheme_id_uri) for ID3 timed metadata in your output. For more information, see ISO/IEC 23009-1:2022 section 5.10.3.3.4 Semantics. Leave blank to use the default value: https://aomedia.org/emsg/ID3 When you specify a value for ID3 metadata scheme ID URI, you must also set ID3 metadata (timedMetadata) to Passthrough.\"\n        }\n      ]\n    },\n    \"TimedMetadataValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMax1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataValue\"\
  \n          },\n          \"description\": \"Specify the event message box (eMSG) value for ID3 timed metadata in your output. For more information, see ISO/IEC 23009-1:2022 section 5.10.3.3.4 Semantics. When you specify a value for ID3 Metadata Value, you must also set ID3 metadata (timedMetadata) to Passthrough.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mpd-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MpdSettings
---
