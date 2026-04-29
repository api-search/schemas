---
description: MPEG-2 TS container settings. These apply to outputs in a File output group when the output's container (ContainerType) is MPEG-2 Transport Stream (M2TS). In these assets, data is organized by the program map table (PMT). Each transport stream program contains subsets of data, including audio, video, and metadata. Each of these subsets of data has a numerical label called a packet identifier (PID). Each transport stream program corresponds to one MediaConvert output. The PMT lists the types of data in a program along with their PID. Downstream systems and players use the program map table to look up the PID for each type of data it accesses and then uses the PIDs to locate specific data within the asset.
layout: schema
name: M2tsSettings
properties_list:
- description: ''
  name: AudioBufferModel
  type: object
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
  name: Bitrate
  type: object
- description: ''
  name: BufferModel
  type: object
- description: ''
  name: DataPTSControl
  type: object
- description: ''
  name: DvbNitSettings
  type: object
- description: ''
  name: DvbSdtSettings
  type: object
- description: ''
  name: DvbSubPids
  type: object
- description: ''
  name: DvbTdtSettings
  type: object
- description: ''
  name: DvbTeletextPid
  type: object
- description: ''
  name: EbpAudioInterval
  type: object
- description: ''
  name: EbpPlacement
  type: object
- description: ''
  name: EsRateInPes
  type: object
- description: ''
  name: ForceTsVideoEbpOrder
  type: object
- description: ''
  name: FragmentTime
  type: object
- description: ''
  name: KlvMetadata
  type: object
- description: ''
  name: MaxPcrInterval
  type: object
- description: ''
  name: MinEbpInterval
  type: object
- description: ''
  name: NielsenId3
  type: object
- description: ''
  name: NullPacketBitrate
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
  name: RateMode
  type: object
- description: ''
  name: Scte35Esam
  type: object
- description: ''
  name: Scte35Pid
  type: object
- description: ''
  name: Scte35Source
  type: object
- description: ''
  name: SegmentationMarkers
  type: object
- description: ''
  name: SegmentationStyle
  type: object
- description: ''
  name: SegmentationTime
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
schema_file: json-schema/mediaconvert-api-m2ts-settings-schema.json
slug: mediaconvert-api-m2ts-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-settings-schema.json\",\n  \"title\": \"M2tsSettings\",\n  \"description\": \"MPEG-2 TS container settings. These apply to outputs in a File output group when the output's container (ContainerType) is MPEG-2 Transport Stream (M2TS). In these assets, data is organized by the program map table (PMT). Each transport stream program contains subsets of data, including audio, video, and metadata. Each of these subsets of data has a numerical label called a packet identifier (PID). Each transport stream program corresponds to one MediaConvert output. The PMT lists the types of data in a program along with their PID. Downstream systems and players use the program map table to look up the PID for each type of data it accesses and then uses the PIDs to locate specific data within the asset.\"\
  ,\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioBufferModel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsAudioBufferModel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioBufferModel\"\n          },\n          \"description\": \"Selects between the DVB and ATSC buffer models for Dolby Digital audio.\"\n        }\n      ]\n    },\n    \"AudioDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsAudioDuration\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioDuration\"\n          },\n          \"description\": \"Specify this setting only when your output will be consumed by a downstream repackaging workflow that is sensitive to very small duration differences between video and audio. For this situation, choose Match video duration (MATCH_VIDEO_DURATION). In all other cases, keep the default value, Default codec duration (DEFAULT_CODEC_DURATION).\
  \ When you choose Match video duration, MediaConvert pads the output audio streams with silence or trims them to ensure that the total duration of each audio stream is at least as long as the total duration of the video stream. After padding or trimming, the audio stream duration is no more than one frame longer than the video stream. MediaConvert applies audio padding or trimming only to the end of the last segment of the output. For unsegmented outputs, MediaConvert adds padding only to the end of the file. When you keep the default value, any minor discrepancies between audio and video duration will depend on your output audio codec.\"\n        }\n      ]\n    },\n    \"AudioFramesPerPes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioFramesPerPes\"\n          },\n          \"description\": \"The number of audio frames to insert for each PES packet.\"\
  \n        }\n      ]\n    },\n    \"AudioPids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioPids\"\n          },\n          \"description\": \"Specify the packet identifiers (PIDs) for any elementary audio streams you include in this output. Specify multiple PIDs as a JSON array. Default is the range 482-492.\"\n        }\n      ]\n    },\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"Specify the output bitrate of the transport stream in bits per second. Setting to 0 lets the muxer automatically determine the appropriate bitrate. Other common values are 3750000, 7500000, and 15000000.\"\n        }\n      ]\n    },\n    \"BufferModel\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/M2tsBufferModel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bufferModel\"\n          },\n          \"description\": \"Controls what buffer model to use for accurate interleaving. If set to MULTIPLEX, use multiplex buffer model. If set to NONE, this can lead to lower latency, but low-memory devices may not be able to play back the stream without interruptions.\"\n        }\n      ]\n    },\n    \"DataPTSControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsDataPtsControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dataPTSControl\"\n          },\n          \"description\": \"If you select ALIGN_TO_VIDEO, MediaConvert writes captions and data packets with Presentation Timestamp (PTS) values greater than or equal to the first video packet PTS (MediaConvert drops captions and data packets with lesser PTS values). Keep the default value (AUTO)\
  \ to allow all PTS values.\"\n        }\n      ]\n    },\n    \"DvbNitSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbNitSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbNitSettings\"\n          },\n          \"description\": \"Use these settings to insert a DVB Network Information Table (NIT) in the transport stream of this output. When you work directly in your JSON job specification, include this object only when your job has a transport stream output and the container settings contain the object M2tsSettings.\"\n        }\n      ]\n    },\n    \"DvbSdtSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbSdtSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbSdtSettings\"\n          },\n          \"description\": \"Use these settings to insert a DVB Service Description Table (SDT) in the transport stream of this output. When you work directly\
  \ in your JSON job specification, include this object only when your job has a transport stream output and the container settings contain the object M2tsSettings.\"\n        }\n      ]\n    },\n    \"DvbSubPids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbSubPids\"\n          },\n          \"description\": \"Specify the packet identifiers (PIDs) for DVB subtitle data included in this output. Specify multiple PIDs as a JSON array. Default is the range 460-479.\"\n        }\n      ]\n    },\n    \"DvbTdtSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbTdtSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbTdtSettings\"\n          },\n          \"description\": \"Use these settings to insert a DVB Time and Date Table (TDT) in the transport stream of this output. When you work directly\
  \ in your JSON job specification, include this object only when your job has a transport stream output and the container settings contain the object M2tsSettings.\"\n        }\n      ]\n    },\n    \"DvbTeletextPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbTeletextPid\"\n          },\n          \"description\": \"Specify the packet identifier (PID) for DVB teletext data you include in this output. Default is 499.\"\n        }\n      ]\n    },\n    \"EbpAudioInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsEbpAudioInterval\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ebpAudioInterval\"\n          },\n          \"description\": \"When set to VIDEO_AND_FIXED_INTERVALS, audio EBP markers will be added to partitions 3 and 4. The interval between these additional markers will be fixed, and\
  \ will be slightly shorter than the video EBP marker interval. When set to VIDEO_INTERVAL, these additional markers will not be inserted. Only applicable when EBP segmentation markers are is selected (segmentationMarkers is EBP or EBP_LEGACY).\"\n        }\n      ]\n    },\n    \"EbpPlacement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsEbpPlacement\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ebpPlacement\"\n          },\n          \"description\": \"Selects which PIDs to place EBP markers on. They can either be placed only on the video PID, or on both the video PID and all audio PIDs. Only applicable when EBP segmentation markers are is selected (segmentationMarkers is EBP or EBP_LEGACY).\"\n        }\n      ]\n    },\n    \"EsRateInPes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsEsRateInPes\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"esRateInPes\"\n \
  \         },\n          \"description\": \"Controls whether to include the ES Rate field in the PES header.\"\n        }\n      ]\n    },\n    \"ForceTsVideoEbpOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsForceTsVideoEbpOrder\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"forceTsVideoEbpOrder\"\n          },\n          \"description\": \"Keep the default value (DEFAULT) unless you know that your audio EBP markers are incorrectly appearing before your video EBP markers. To correct this problem, set this value to Force (FORCE).\"\n        }\n      ]\n    },\n    \"FragmentTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fragmentTime\"\n          },\n          \"description\": \"The length, in seconds, of each fragment. Only used with EBP markers.\"\n        }\n      ]\n    },\n    \"KlvMetadata\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsKlvMetadata\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"klvMetadata\"\n          },\n          \"description\": \"To include key-length-value metadata in this output: Set KLV metadata insertion to Passthrough. MediaConvert reads KLV metadata present in your input and passes it through to the output transport stream. To exclude this KLV metadata: Set KLV metadata insertion to None or leave blank.\"\n        }\n      ]\n    },\n    \"MaxPcrInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max500\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxPcrInterval\"\n          },\n          \"description\": \"Specify the maximum time, in milliseconds, between Program Clock References (PCRs) inserted into the transport stream.\"\n        }\n      ]\n    },\n    \"MinEbpInterval\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/__integerMin0Max10000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minEbpInterval\"\n          },\n          \"description\": \"When set, enforces that Encoder Boundary Points do not come within the specified time interval of each other by looking ahead at input video. If another EBP is going to come in within the specified time interval, the current EBP is not emitted, and the segment is \\\"stretched\\\" to the next marker. The lookahead value does not add latency to the system. The Live Event must be configured elsewhere to create sufficient latency to make the lookahead accurate.\"\n        }\n      ]\n    },\n    \"NielsenId3\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsNielsenId3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nielsenId3\"\n          },\n          \"description\": \"If INSERT, Nielsen inaudible tones for media tracking will be detected\
  \ in the input audio and an equivalent ID3 tag will be inserted in the output.\"\n        }\n      ]\n    },\n    \"NullPacketBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nullPacketBitrate\"\n          },\n          \"description\": \"Value in bits per second of extra null packets to insert into the transport stream. This can be used if a downstream encryption system requires periodic null packets.\"\n        }\n      ]\n    },\n    \"PatInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"patInterval\"\n          },\n          \"description\": \"The number of milliseconds between instances of this table in the output transport stream.\"\n        }\n      ]\n    },\n    \"PcrControl\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/M2tsPcrControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pcrControl\"\n          },\n          \"description\": \"When set to PCR_EVERY_PES_PACKET, a Program Clock Reference value is inserted for every Packetized Elementary Stream (PES) header. This is effective only when the PCR PID is the same as the video or audio elementary stream.\"\n        }\n      ]\n    },\n    \"PcrPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pcrPid\"\n          },\n          \"description\": \"Specify the packet identifier (PID) for the program clock reference (PCR) in this output. If you do not specify a value, the service will use the value for Video PID (VideoPid).\"\n        }\n      ]\n    },\n    \"PmtInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max1000\"\n    \
  \    },\n        {\n          \"xml\": {\n            \"name\": \"pmtInterval\"\n          },\n          \"description\": \"Specify the number of milliseconds between instances of the program map table (PMT) in the output transport stream.\"\n        }\n      ]\n    },\n    \"PmtPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pmtPid\"\n          },\n          \"description\": \"Specify the packet identifier (PID) for the program map table (PMT) itself. Default is 480.\"\n        }\n      ]\n    },\n    \"PrivateMetadataPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"privateMetadataPid\"\n          },\n          \"description\": \"Specify the packet identifier (PID) of the private metadata stream. Default is 503.\"\n        }\n   \
  \   ]\n    },\n    \"ProgramNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65535\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programNumber\"\n          },\n          \"description\": \"Use Program number (programNumber) to specify the program number used in the program map table (PMT) for this output. Default is 1. Program numbers and program map tables are parts of MPEG-2 transport stream containers, used for organizing data.\"\n        }\n      ]\n    },\n    \"RateMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsRateMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rateMode\"\n          },\n          \"description\": \"When set to CBR, inserts null packets into transport stream to fill specified bitrate. When set to VBR, the bitrate setting acts as the maximum bitrate, but the output will not be padded up to that bitrate.\"\n        }\n\
  \      ]\n    },\n    \"Scte35Esam\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsScte35Esam\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35Esam\"\n          },\n          \"description\": \"Include this in your job settings to put SCTE-35 markers in your HLS and transport stream outputs at the insertion points that you specify in an ESAM XML document. Provide the document in the setting SCC XML (sccXml).\"\n        }\n      ]\n    },\n    \"Scte35Pid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35Pid\"\n          },\n          \"description\": \"Specify the packet identifier (PID) of the SCTE-35 stream in the transport stream.\"\n        }\n      ]\n    },\n    \"Scte35Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsScte35Source\"\n        },\n\
  \        {\n          \"xml\": {\n            \"name\": \"scte35Source\"\n          },\n          \"description\": \"For SCTE-35 markers from your input-- Choose Passthrough (PASSTHROUGH) if you want SCTE-35 markers that appear in your input to also appear in this output. Choose None (NONE) if you don't want SCTE-35 markers in this output. For SCTE-35 markers from an ESAM XML document-- Choose None (NONE). Also provide the ESAM XML as a string in the setting Signal processing notification XML (sccXml). Also enable ESAM SCTE-35 (include the property scte35Esam).\"\n        }\n      ]\n    },\n    \"SegmentationMarkers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsSegmentationMarkers\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentationMarkers\"\n          },\n          \"description\": \"Inserts segmentation markers at each segmentation_time period. rai_segstart sets the Random Access Indicator bit in the adaptation field.\
  \ rai_adapt sets the RAI bit and adds the current timecode in the private data bytes. psi_segstart inserts PAT and PMT tables at the start of segments. ebp adds Encoder Boundary Point information to the adaptation field as per OpenCable specification OC-SP-EBP-I01-130118. ebp_legacy adds Encoder Boundary Point information to the adaptation field using a legacy proprietary format.\"\n        }\n      ]\n    },\n    \"SegmentationStyle\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsSegmentationStyle\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentationStyle\"\n          },\n          \"description\": \"The segmentation style parameter controls how segmentation markers are inserted into the transport stream. With avails, it is possible that segments may be truncated, which can influence where future segmentation markers are inserted. When a segmentation style of \\\"reset_cadence\\\" is selected and a segment is truncated\
  \ due to an avail, we will reset the segmentation cadence. This means the subsequent segment will have a duration of of $segmentation_time seconds. When a segmentation style of \\\"maintain_cadence\\\" is selected and a segment is truncated due to an avail, we will not reset the segmentation cadence. This means the subsequent segment will likely be truncated as well. However, all segments after that will have a duration of $segmentation_time seconds. Note that EBP lookahead is a slight exception to this rule.\"\n        }\n      ]\n    },\n    \"SegmentationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentationTime\"\n          },\n          \"description\": \"Specify the length, in seconds, of each segment. Required unless markers is set to _none_.\"\n        }\n      ]\n    },\n    \"TimedMetadataPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataPid\"\n          },\n          \"description\": \"Packet Identifier (PID) of the ID3 metadata stream in the transport stream.\"\n        }\n      ]\n    },\n    \"TransportStreamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65535\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"transportStreamId\"\n          },\n          \"description\": \"Specify the ID for the transport stream itself in the program map table for this output. Transport stream IDs and program map tables are parts of MPEG-2 transport stream containers, used for organizing data.\"\n        }\n      ]\n    },\n    \"VideoPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8182\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoPid\"\n          },\n\
  \          \"description\": \"Specify the packet identifier (PID) of the elementary video stream in the transport stream.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: M2tsSettings
---
