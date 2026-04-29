---
description: Settings information for the .m3u8 container
layout: schema
name: M3u8Settings
properties_list:
- description: ''
  name: AudioFramesPerPes
  type: object
- description: ''
  name: AudioPids
  type: object
- description: ''
  name: EcmPid
  type: object
- description: ''
  name: NielsenId3Behavior
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
  name: Scte35Behavior
  type: object
- description: ''
  name: Scte35Pid
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
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-m3u8-settings-schema.json
slug: medialive-api-m3u8-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-m3u8-settings-schema.json\",\n  \"title\": \"M3u8Settings\",\n  \"description\": \"Settings information for the .m3u8 container\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioFramesPerPes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioFramesPerPes\"\n          },\n          \"description\": \"The number of audio frames to insert for each PES packet.\"\n        }\n      ]\n    },\n    \"AudioPids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioPids\"\n          },\n          \"description\": \"Packet Identifier (PID) of the elementary audio\
  \ stream(s) in the transport stream. Multiple values are accepted, and can be entered in ranges and/or by comma separation. Can be entered as decimal or hexadecimal values.\"\n        }\n      ]\n    },\n    \"EcmPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ecmPid\"\n          },\n          \"description\": \"This parameter is unused and deprecated.\"\n        }\n      ]\n    },\n    \"NielsenId3Behavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M3u8NielsenId3Behavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nielsenId3Behavior\"\n          },\n          \"description\": \"If set to passthrough, Nielsen inaudible tones for media tracking will be detected in the input audio and an equivalent ID3 tag will be inserted in the output.\"\n        }\n      ]\n    },\n    \"PatInterval\": {\n      \"allOf\":\
  \ [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"patInterval\"\n          },\n          \"description\": \"The number of milliseconds between instances of this table in the output transport stream. A value of \\\\\\\"0\\\\\\\" writes out the PMT once per segment file.\"\n        }\n      ]\n    },\n    \"PcrControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M3u8PcrControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pcrControl\"\n          },\n          \"description\": \"When set to pcrEveryPesPacket, a Program Clock Reference value is inserted for every Packetized Elementary Stream (PES) header. This parameter is effective only when the PCR PID is the same as the video or audio elementary stream.\"\n        }\n      ]\n    },\n    \"PcrPeriod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max500\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"pcrPeriod\"\n          },\n          \"description\": \"Maximum time in milliseconds between Program Clock References (PCRs) inserted into the transport stream.\"\n        }\n      ]\n    },\n    \"PcrPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pcrPid\"\n          },\n          \"description\": \"Packet Identifier (PID) of the Program Clock Reference (PCR) in the transport stream. When no value is given, the encoder will assign the same value as the Video PID. Can be entered as a decimal or hexadecimal value.\"\n        }\n      ]\n    },\n    \"PmtInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pmtInterval\"\n          },\n          \"description\": \"The number of\
  \ milliseconds between instances of this table in the output transport stream. A value of \\\\\\\"0\\\\\\\" writes out the PMT once per segment file.\"\n        }\n      ]\n    },\n    \"PmtPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pmtPid\"\n          },\n          \"description\": \"Packet Identifier (PID) for the Program Map Table (PMT) in the transport stream. Can be entered as a decimal or hexadecimal value.\"\n        }\n      ]\n    },\n    \"ProgramNum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65535\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programNum\"\n          },\n          \"description\": \"The value of the program number field in the Program Map Table.\"\n        }\n      ]\n    },\n    \"Scte35Behavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M3u8Scte35Behavior\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35Behavior\"\n          },\n          \"description\": \"If set to passthrough, passes any SCTE-35 signals from the input source to this output.\"\n        }\n      ]\n    },\n    \"Scte35Pid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35Pid\"\n          },\n          \"description\": \"Packet Identifier (PID) of the SCTE-35 stream in the transport stream. Can be entered as a decimal or hexadecimal value.\"\n        }\n      ]\n    },\n    \"TimedMetadataBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M3u8TimedMetadataBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataBehavior\"\n          },\n          \"description\": \"When set to passthrough, timed metadata is passed through from input to output.\"\n      \
  \  }\n      ]\n    },\n    \"TimedMetadataPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataPid\"\n          },\n          \"description\": \"Packet Identifier (PID) of the timed metadata stream in the transport stream. Can be entered as a decimal or hexadecimal value.  Valid values are 32 (or 0x20)..8182 (or 0x1ff6).\"\n        }\n      ]\n    },\n    \"TransportStreamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max65535\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"transportStreamId\"\n          },\n          \"description\": \"The value of the transport stream ID field in the Program Map Table.\"\n        }\n      ]\n    },\n    \"VideoPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n      \
  \      \"name\": \"videoPid\"\n          },\n          \"description\": \"Packet Identifier (PID) of the elementary video stream in the transport stream. Can be entered as a decimal or hexadecimal value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-m3u8-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: M3u8Settings
---
