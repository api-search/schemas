---
description: These settings relate to the MPEG-2 transport stream (MPEG2-TS) container for the MPEG2-TS segments in your HLS outputs.
layout: schema
name: M3u8Settings
properties_list:
- description: ''
  name: AudioDuration
  type: object
- description: ''
  name: AudioFramesPerPes
  type: object
- description: ''
  name: AudioPids
  type: object
- description: ''
  name: DataPTSControl
  type: object
- description: ''
  name: MaxPcrInterval
  type: object
- description: ''
  name: NielsenId3
  type: object
- description: ''
  name: PatInterval
  type: object
- description: ''
  name: PcrControl
  type: object
- description: ''
  name: PcrPid
  type: object
- description: ''
  name: PmtInterval
  type: object
- description: ''
  name: PmtPid
  type: object
- description: ''
  name: PrivateMetadataPid
  type: object
- description: ''
  name: ProgramNumber
  type: object
- description: ''
  name: Scte35Pid
  type: object
- description: ''
  name: Scte35Source
  type: object
- description: ''
  name: TimedMetadata
  type: object
- description: ''
  name: TimedMetadataPid
  type: object
- description: ''
  name: TransportStreamId
  type: object
- description: ''
  name: VideoPid
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-m3u8-settings-schema.json
slug: mediaconvert-api-m3u8-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m3u8-settings-schema.json\",\n  \"title\": \"M3u8Settings\",\n  \"description\": \"These settings relate to the MPEG-2 transport stream (MPEG2-TS) container for the MPEG2-TS segments in your HLS outputs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M3u8AudioDuration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioDuration\"\n          },\n          \"description\": \"Specify this setting only when your output will be consumed by a downstream repackaging workflow that is sensitive to very small duration differences between video and audio. For this situation, choose Match video duration (MATCH_VIDEO_DURATION). In all other cases, keep the default value,\
  \ Default codec duration (DEFAULT_CODEC_DURATION). When you choose Match video duration, MediaConvert pads the output audio streams with silence or trims them to ensure that the total duration of each audio stream is at least as long as the total duration of the video stream. After padding or trimming, the audio stream duration is no more than one frame longer than the video stream. MediaConvert applies audio padding or trimming only to the end of the last segment of the output. For unsegmented outputs, MediaConvert adds padding only to the end of the file. When you keep the default value, any minor discrepancies between audio and video duration will depend on your output audio codec.\"\n        }\n      ]\n    },\n    \"AudioFramesPerPes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioFramesPerPes\"\n          },\n          \"description\": \"The number\
  \ of audio frames to insert for each PES packet.\"\n        }\n      ]\n    },\n    \"AudioPids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioPids\"\n          },\n          \"description\": \"Packet Identifier (PID) of the elementary audio stream(s) in the transport stream. Multiple values are accepted, and can be entered in ranges and/or by comma separation.\"\n        }\n      ]\n    },\n    \"DataPTSControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M3u8DataPtsControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dataPTSControl\"\n          },\n          \"description\": \"If you select ALIGN_TO_VIDEO, MediaConvert writes captions and data packets with Presentation Timestamp (PTS) values greater than or equal to the first video packet PTS (MediaConvert drops captions and data packets\
  \ with lesser PTS values). Keep the default value (AUTO) to allow all PTS values.\"\n        }\n      ]\n    },\n    \"MaxPcrInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max500\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxPcrInterval\"\n          },\n          \"description\": \"Specify the maximum time, in milliseconds, between Program Clock References (PCRs) inserted into the transport stream.\"\n        }\n      ]\n    },\n    \"NielsenId3\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M3u8NielsenId3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nielsenId3\"\n          },\n          \"description\": \"If INSERT, Nielsen inaudible tones for media tracking will be detected in the input audio and an equivalent ID3 tag will be inserted in the output.\"\n        }\n      ]\n    },\n    \"PatInterval\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/__integerMin0Max1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"patInterval\"\n          },\n          \"description\": \"The number of milliseconds between instances of this table in the output transport stream.\"\n        }\n      ]\n    },\n    \"PcrControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M3u8PcrControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pcrControl\"\n          },\n          \"description\": \"When set to PCR_EVERY_PES_PACKET a Program Clock Reference value is inserted for every Packetized Elementary Stream (PES) header. This parameter is effective only when the PCR PID is the same as the video or audio elementary stream.\"\n        }\n      ]\n    },\n    \"PcrPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\":\
  \ \"pcrPid\"\n          },\n          \"description\": \"Packet Identifier (PID) of the Program Clock Reference (PCR) in the transport stream. When no value is given, the encoder will assign the same value as the Video PID.\"\n        }\n      ]\n    },\n    \"PmtInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pmtInterval\"\n          },\n          \"description\": \"The number of milliseconds between instances of this table in the output transport stream.\"\n        }\n      ]\n    },\n    \"PmtPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pmtPid\"\n          },\n          \"description\": \"Packet Identifier (PID) for the Program Map Table (PMT) in the transport stream.\"\n        }\n      ]\n    },\n    \"PrivateMetadataPid\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"privateMetadataPid\"\n          },\n          \"description\": \"Packet Identifier (PID) of the private metadata stream in the transport stream.\"\n        }\n      ]\n    },\n    \"ProgramNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65535\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programNumber\"\n          },\n          \"description\": \"The value of the program number field in the Program Map Table.\"\n        }\n      ]\n    },\n    \"Scte35Pid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35Pid\"\n          },\n          \"description\": \"Packet Identifier (PID) of the SCTE-35 stream in the transport\
  \ stream.\"\n        }\n      ]\n    },\n    \"Scte35Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M3u8Scte35Source\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35Source\"\n          },\n          \"description\": \"For SCTE-35 markers from your input-- Choose Passthrough (PASSTHROUGH) if you want SCTE-35 markers that appear in your input to also appear in this output. Choose None (NONE) if you don't want SCTE-35 markers in this output. For SCTE-35 markers from an ESAM XML document-- Choose None (NONE) if you don't want manifest conditioning. Choose Passthrough (PASSTHROUGH) and choose Ad markers (adMarkers) if you do want manifest conditioning. In both cases, also provide the ESAM XML as a string in the setting Signal processing notification XML (sccXml).\"\n        }\n      ]\n    },\n    \"TimedMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimedMetadata\"\n        },\n\
  \        {\n          \"xml\": {\n            \"name\": \"timedMetadata\"\n          },\n          \"description\": \"Set ID3 metadata (timedMetadata) to Passthrough (PASSTHROUGH) to include ID3 metadata in this output. This includes ID3 metadata from the following features: ID3 timestamp period (timedMetadataId3Period), and Custom ID3 metadata inserter (timedMetadataInsertion). To exclude this ID3 metadata in this output: set ID3 metadata to None (NONE) or leave blank.\"\n        }\n      ]\n    },\n    \"TimedMetadataPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataPid\"\n          },\n          \"description\": \"Packet Identifier (PID) of the ID3 metadata stream in the transport stream.\"\n        }\n      ]\n    },\n    \"TransportStreamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65535\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"transportStreamId\"\n          },\n          \"description\": \"The value of the transport stream ID field in the Program Map Table.\"\n        }\n      ]\n    },\n    \"VideoPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoPid\"\n          },\n          \"description\": \"Packet Identifier (PID) of the elementary video stream in the transport stream.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m3u8-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: M3u8Settings
---
