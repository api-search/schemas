---
description: M2ts Settings
layout: schema
name: M2tsSettings
properties_list:
- description: ''
  name: AbsentInputAudioBehavior
  type: object
- description: ''
  name: Arib
  type: object
- description: ''
  name: AribCaptionsPid
  type: object
- description: ''
  name: AribCaptionsPidControl
  type: object
- description: ''
  name: AudioBufferModel
  type: object
- description: ''
  name: AudioFramesPerPes
  type: object
- description: ''
  name: AudioPids
  type: object
- description: ''
  name: AudioStreamType
  type: object
- description: ''
  name: Bitrate
  type: object
- description: ''
  name: BufferModel
  type: object
- description: ''
  name: CcDescriptor
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
  name: Ebif
  type: object
- description: ''
  name: EbpAudioInterval
  type: object
- description: ''
  name: EbpLookaheadMs
  type: object
- description: ''
  name: EbpPlacement
  type: object
- description: ''
  name: EcmPid
  type: object
- description: ''
  name: EsRateInPes
  type: object
- description: ''
  name: EtvPlatformPid
  type: object
- description: ''
  name: EtvSignalPid
  type: object
- description: ''
  name: FragmentTime
  type: object
- description: ''
  name: Klv
  type: object
- description: ''
  name: KlvDataPids
  type: object
- description: ''
  name: NielsenId3Behavior
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
  name: PcrPeriod
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
  name: ProgramNum
  type: object
- description: ''
  name: RateMode
  type: object
- description: ''
  name: Scte27Pids
  type: object
- description: ''
  name: Scte35Control
  type: object
- description: ''
  name: Scte35Pid
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
  name: TimedMetadataBehavior
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
- description: ''
  name: Scte35PrerollPullupMilliseconds
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-m2ts-settings-schema.json
slug: medialive-api-m2ts-settings
source_filename: medialive-api-m2ts-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-m2ts-settings-schema.json\",\n  \"title\": \"M2tsSettings\",\n  \"description\": \"M2ts Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AbsentInputAudioBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsAbsentInputAudioBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"absentInputAudioBehavior\"\n          },\n          \"description\": \"When set to drop, output audio streams will be removed from the program if the selected input audio stream is removed from the input. This allows the output audio configuration to dynamically change based on input configuration. If this is set to encodeSilence, all output audio streams will output encoded silence when not connected to an active input stream.\"\n   \
  \     }\n      ]\n    },\n    \"Arib\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsArib\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arib\"\n          },\n          \"description\": \"When set to enabled, uses ARIB-compliant field muxing and removes video descriptor.\"\n        }\n      ]\n    },\n    \"AribCaptionsPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"aribCaptionsPid\"\n          },\n          \"description\": \"Packet Identifier (PID) for ARIB Captions in the transport stream. Can be entered as a decimal or hexadecimal value.  Valid values are 32 (or 0x20)..8182 (or 0x1ff6).\"\n        }\n      ]\n    },\n    \"AribCaptionsPidControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsAribCaptionsPidControl\"\n        },\n        {\n          \"xml\": {\n        \
  \    \"name\": \"aribCaptionsPidControl\"\n          },\n          \"description\": \"If set to auto, pid number used for ARIB Captions will be auto-selected from unused pids.  If set to useConfigured, ARIB Captions will be on the configured pid number.\"\n        }\n      ]\n    },\n    \"AudioBufferModel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsAudioBufferModel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioBufferModel\"\n          },\n          \"description\": \"When set to dvb, uses DVB buffer model for Dolby Digital audio.  When set to atsc, the ATSC model is used.\"\n        }\n      ]\n    },\n    \"AudioFramesPerPes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioFramesPerPes\"\n          },\n          \"description\": \"The number of audio frames to insert for each PES packet.\"\n  \
  \      }\n      ]\n    },\n    \"AudioPids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioPids\"\n          },\n          \"description\": \"Packet Identifier (PID) of the elementary audio stream(s) in the transport stream. Multiple values are accepted, and can be entered in ranges and/or by comma separation. Can be entered as decimal or hexadecimal values. Each PID specified must be in the range of 32 (or 0x20)..8182 (or 0x1ff6).\"\n        }\n      ]\n    },\n    \"AudioStreamType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsAudioStreamType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioStreamType\"\n          },\n          \"description\": \"When set to atsc, uses stream type = 0x81 for AC3 and stream type = 0x87 for EAC3. When set to dvb, uses stream type = 0x06.\"\n        }\n      ]\n    },\n  \
  \  \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"The output bitrate of the transport stream in bits per second. Setting to 0 lets the muxer automatically determine the appropriate bitrate.\"\n        }\n      ]\n    },\n    \"BufferModel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsBufferModel\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bufferModel\"\n          },\n          \"description\": \"Controls the timing accuracy for output network traffic. Leave as MULTIPLEX to ensure accurate network packet timing. Or set to NONE, which might result in lower latency but will result in more variability in output network packet timing. This variability might cause interruptions, jitter, or bursty behavior in your playback or receiving devices.\"\n\
  \        }\n      ]\n    },\n    \"CcDescriptor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsCcDescriptor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ccDescriptor\"\n          },\n          \"description\": \"When set to enabled, generates captionServiceDescriptor in PMT.\"\n        }\n      ]\n    },\n    \"DvbNitSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbNitSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbNitSettings\"\n          },\n          \"description\": \"Inserts DVB Network Information Table (NIT) at the specified table repetition interval.\"\n        }\n      ]\n    },\n    \"DvbSdtSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbSdtSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbSdtSettings\"\n          },\n          \"description\": \"Inserts DVB\
  \ Service Description Table (SDT) at the specified table repetition interval.\"\n        }\n      ]\n    },\n    \"DvbSubPids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbSubPids\"\n          },\n          \"description\": \"Packet Identifier (PID) for input source DVB Subtitle data to this output. Multiple values are accepted, and can be entered in ranges and/or by comma separation. Can be entered as decimal or hexadecimal values.  Each PID specified must be in the range of 32 (or 0x20)..8182 (or 0x1ff6).\"\n        }\n      ]\n    },\n    \"DvbTdtSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbTdtSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbTdtSettings\"\n          },\n          \"description\": \"Inserts DVB Time and Date Table (TDT) at the specified table repetition interval.\"\n   \
  \     }\n      ]\n    },\n    \"DvbTeletextPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbTeletextPid\"\n          },\n          \"description\": \"Packet Identifier (PID) for input source DVB Teletext data to this output. Can be entered as a decimal or hexadecimal value.  Valid values are 32 (or 0x20)..8182 (or 0x1ff6).\"\n        }\n      ]\n    },\n    \"Ebif\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsEbifControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ebif\"\n          },\n          \"description\": \"If set to passthrough, passes any EBIF data from the input source to this output.\"\n        }\n      ]\n    },\n    \"EbpAudioInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsAudioInterval\"\n        },\n        {\n          \"xml\": {\n            \"\
  name\": \"ebpAudioInterval\"\n          },\n          \"description\": \"When videoAndFixedIntervals is selected, audio EBP markers will be added to partitions 3 and 4. The interval between these additional markers will be fixed, and will be slightly shorter than the video EBP marker interval. Only available when EBP Cablelabs segmentation markers are selected.  Partitions 1 and 2 will always follow the video interval.\"\n        }\n      ]\n    },\n    \"EbpLookaheadMs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max10000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ebpLookaheadMs\"\n          },\n          \"description\": \"When set, enforces that Encoder Boundary Points do not come within the specified time interval of each other by looking ahead at input video. If another EBP is going to come in within the specified time interval, the current EBP is not emitted, and the segment is \\\"stretched\\\" to the next\
  \ marker.  The lookahead value does not add latency to the system. The Live Event must be configured elsewhere to create sufficient latency to make the lookahead accurate.\"\n        }\n      ]\n    },\n    \"EbpPlacement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsEbpPlacement\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ebpPlacement\"\n          },\n          \"description\": \"Controls placement of EBP on Audio PIDs. If set to videoAndAudioPids, EBP markers will be placed on the video PID and all audio PIDs.  If set to videoPid, EBP markers will be placed on only the video PID.\"\n        }\n      ]\n    },\n    \"EcmPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ecmPid\"\n          },\n          \"description\": \"This field is unused and deprecated.\"\n        }\n      ]\n    },\n    \"EsRateInPes\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsEsRateInPes\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"esRateInPes\"\n          },\n          \"description\": \"Include or exclude the ES Rate field in the PES header.\"\n        }\n      ]\n    },\n    \"EtvPlatformPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"etvPlatformPid\"\n          },\n          \"description\": \"Packet Identifier (PID) for input source ETV Platform data to this output. Can be entered as a decimal or hexadecimal value.  Valid values are 32 (or 0x20)..8182 (or 0x1ff6).\"\n        }\n      ]\n    },\n    \"EtvSignalPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"etvSignalPid\"\n          },\n          \"description\": \"\
  Packet Identifier (PID) for input source ETV Signal data to this output. Can be entered as a decimal or hexadecimal value.  Valid values are 32 (or 0x20)..8182 (or 0x1ff6).\"\n        }\n      ]\n    },\n    \"FragmentTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fragmentTime\"\n          },\n          \"description\": \"The length in seconds of each fragment. Only used with EBP markers.\"\n        }\n      ]\n    },\n    \"Klv\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsKlv\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"klv\"\n          },\n          \"description\": \"If set to passthrough, passes any KLV data from the input source to this output.\"\n        }\n      ]\n    },\n    \"KlvDataPids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n\
  \        {\n          \"xml\": {\n            \"name\": \"klvDataPids\"\n          },\n          \"description\": \"Packet Identifier (PID) for input source KLV data to this output. Multiple values are accepted, and can be entered in ranges and/or by comma separation. Can be entered as decimal or hexadecimal values.  Each PID specified must be in the range of 32 (or 0x20)..8182 (or 0x1ff6).\"\n        }\n      ]\n    },\n    \"NielsenId3Behavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsNielsenId3Behavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nielsenId3Behavior\"\n          },\n          \"description\": \"If set to passthrough, Nielsen inaudible tones for media tracking will be detected in the input audio and an equivalent ID3 tag will be inserted in the output.\"\n        }\n      ]\n    },\n    \"NullPacketBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0\"\n\
  \        },\n        {\n          \"xml\": {\n            \"name\": \"nullPacketBitrate\"\n          },\n          \"description\": \"Value in bits per second of extra null packets to insert into the transport stream. This can be used if a downstream encryption system requires periodic null packets.\"\n        }\n      ]\n    },\n    \"PatInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"patInterval\"\n          },\n          \"description\": \"The number of milliseconds between instances of this table in the output transport stream.  Valid values are 0, 10..1000.\"\n        }\n      ]\n    },\n    \"PcrControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsPcrControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pcrControl\"\n          },\n          \"description\": \"When set to pcrEveryPesPacket,\
  \ a Program Clock Reference value is inserted for every Packetized Elementary Stream (PES) header. This parameter is effective only when the PCR PID is the same as the video or audio elementary stream.\"\n        }\n      ]\n    },\n    \"PcrPeriod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max500\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pcrPeriod\"\n          },\n          \"description\": \"Maximum time in milliseconds between Program Clock Reference (PCRs) inserted into the transport stream.\"\n        }\n      ]\n    },\n    \"PcrPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pcrPid\"\n          },\n          \"description\": \"Packet Identifier (PID) of the Program Clock Reference (PCR) in the transport stream. When no value is given, the encoder will assign the same value as the Video\
  \ PID. Can be entered as a decimal or hexadecimal value.  Valid values are 32 (or 0x20)..8182 (or 0x1ff6).\"\n        }\n      ]\n    },\n    \"PmtInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pmtInterval\"\n          },\n          \"description\": \"The number of milliseconds between instances of this table in the output transport stream. Valid values are 0, 10..1000.\"\n        }\n      ]\n    },\n    \"PmtPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pmtPid\"\n          },\n          \"description\": \"Packet Identifier (PID) for the Program Map Table (PMT) in the transport stream. Can be entered as a decimal or hexadecimal value. Valid values are 32 (or 0x20)..8182 (or 0x1ff6).\"\n        }\n      ]\n    },\n    \"ProgramNum\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65535\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programNum\"\n          },\n          \"description\": \"The value of the program number field in the Program Map Table.\"\n        }\n      ]\n    },\n    \"RateMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsRateMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rateMode\"\n          },\n          \"description\": \"When vbr, does not insert null packets into transport stream to fill specified bitrate. The bitrate setting acts as the maximum bitrate when vbr is set.\"\n        }\n      ]\n    },\n    \"Scte27Pids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte27Pids\"\n          },\n          \"description\": \"Packet Identifier (PID) for\
  \ input source SCTE-27 data to this output. Multiple values are accepted, and can be entered in ranges and/or by comma separation. Can be entered as decimal or hexadecimal values.  Each PID specified must be in the range of 32 (or 0x20)..8182 (or 0x1ff6).\"\n        }\n      ]\n    },\n    \"Scte35Control\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsScte35Control\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35Control\"\n          },\n          \"description\": \"Optionally pass SCTE-35 signals from the input source to this output.\"\n        }\n      ]\n    },\n    \"Scte35Pid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35Pid\"\n          },\n          \"description\": \"Packet Identifier (PID) of the SCTE-35 stream in the transport stream. Can be entered as a decimal or hexadecimal value.  Valid values\
  \ are 32 (or 0x20)..8182 (or 0x1ff6).\"\n        }\n      ]\n    },\n    \"SegmentationMarkers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsSegmentationMarkers\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentationMarkers\"\n          },\n          \"description\": \"Inserts segmentation markers at each segmentationTime period. raiSegstart sets the Random Access Indicator bit in the adaptation field. raiAdapt sets the RAI bit and adds the current timecode in the private data bytes. psiSegstart inserts PAT and PMT tables at the start of segments. ebp adds Encoder Boundary Point information to the adaptation field as per OpenCable specification OC-SP-EBP-I01-130118. ebpLegacy adds Encoder Boundary Point information to the adaptation field using a legacy proprietary format.\"\n        }\n      ]\n    },\n    \"SegmentationStyle\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsSegmentationStyle\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentationStyle\"\n          },\n          \"description\": \"The segmentation style parameter controls how segmentation markers are inserted into the transport stream. With avails, it is possible that segments may be truncated, which can influence where future segmentation markers are inserted.\\n\\nWhen a segmentation style of \\\"resetCadence\\\" is selected and a segment is truncated due to an avail, we will reset the segmentation cadence. This means the subsequent segment will have a duration of $segmentationTime seconds.\\n\\nWhen a segmentation style of \\\"maintainCadence\\\" is selected and a segment is truncated due to an avail, we will not reset the segmentation cadence. This means the subsequent segment will likely be truncated as well. However, all segments after that will have a duration of $segmentationTime seconds. Note that EBP lookahead is a slight exception to this rule.\"\n        }\n      ]\n\
  \    },\n    \"SegmentationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentationTime\"\n          },\n          \"description\": \"The length in seconds of each segment. Required unless markers is set to _none_.\"\n        }\n      ]\n    },\n    \"TimedMetadataBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsTimedMetadataBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataBehavior\"\n          },\n          \"description\": \"When set to passthrough, timed metadata will be passed through from input to output.\"\n        }\n      ]\n    },\n    \"TimedMetadataPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataPid\"\n          },\n          \"description\"\
  : \"Packet Identifier (PID) of the timed metadata stream in the transport stream. Can be entered as a decimal or hexadecimal value.  Valid values are 32 (or 0x20)..8182 (or 0x1ff6).\"\n        }\n      ]\n    },\n    \"TransportStreamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65535\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"transportStreamId\"\n          },\n          \"description\": \"The value of the transport stream ID field in the Program Map Table.\"\n        }\n      ]\n    },\n    \"VideoPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoPid\"\n          },\n          \"description\": \"Packet Identifier (PID) of the elementary video stream in the transport stream. Can be entered as a decimal or hexadecimal value.  Valid values are 32 (or 0x20)..8182 (or 0x1ff6).\"\n        }\n\
  \      ]\n    },\n    \"Scte35PrerollPullupMilliseconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__doubleMin0Max5000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35PrerollPullupMilliseconds\"\n          },\n          \"description\": \"Defines the amount SCTE-35 preroll will be increased (in milliseconds) on the output. Preroll is the amount of time between the presence of a SCTE-35 indication in a transport stream and the PTS of the video frame it references. Zero means don't add pullup (it doesn't mean set the preroll to zero). Negative pullup is not supported, which means that you can't make the preroll shorter. Be aware that latency in the output will increase by the pullup amount.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-m2ts-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: M2tsSettings
---
