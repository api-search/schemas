---
description: Packet identifiers map for a given Multiplex program.
layout: schema
name: MultiplexProgramPacketIdentifiersMap
properties_list:
- description: ''
  name: AudioPids
  type: object
- description: ''
  name: DvbSubPids
  type: object
- description: ''
  name: DvbTeletextPid
  type: object
- description: ''
  name: EtvPlatformPid
  type: object
- description: ''
  name: EtvSignalPid
  type: object
- description: ''
  name: KlvDataPids
  type: object
- description: ''
  name: PcrPid
  type: object
- description: ''
  name: PmtPid
  type: object
- description: ''
  name: PrivateMetadataPid
  type: object
- description: ''
  name: Scte27Pids
  type: object
- description: ''
  name: Scte35Pid
  type: object
- description: ''
  name: TimedMetadataPid
  type: object
- description: ''
  name: VideoPid
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-multiplex-program-packet-identifiers-map-schema.json
slug: medialive-api-multiplex-program-packet-identifiers-map
source_filename: medialive-api-multiplex-program-packet-identifiers-map-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-program-packet-identifiers-map-schema.json\",\n  \"title\": \"MultiplexProgramPacketIdentifiersMap\",\n  \"description\": \"Packet identifiers map for a given Multiplex program.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioPids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioPids\"\n          }\n        }\n      ]\n    },\n    \"DvbSubPids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbSubPids\"\n          }\n        }\n      ]\n    },\n    \"DvbTeletextPid\": {\n      \"allOf\": [\n        {\n          \"$ref\":\
  \ \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dvbTeletextPid\"\n          }\n        }\n      ]\n    },\n    \"EtvPlatformPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"etvPlatformPid\"\n          }\n        }\n      ]\n    },\n    \"EtvSignalPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"etvSignalPid\"\n          }\n        }\n      ]\n    },\n    \"KlvDataPids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"klvDataPids\"\n          }\n        }\n      ]\n    },\n    \"PcrPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n   \
  \     },\n        {\n          \"xml\": {\n            \"name\": \"pcrPid\"\n          }\n        }\n      ]\n    },\n    \"PmtPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pmtPid\"\n          }\n        }\n      ]\n    },\n    \"PrivateMetadataPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"privateMetadataPid\"\n          }\n        }\n      ]\n    },\n    \"Scte27Pids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte27Pids\"\n          }\n        }\n      ]\n    },\n    \"Scte35Pid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n         \
  \   \"name\": \"scte35Pid\"\n          }\n        }\n      ]\n    },\n    \"TimedMetadataPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"timedMetadataPid\"\n          }\n        }\n      ]\n    },\n    \"VideoPid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoPid\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-program-packet-identifiers-map-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MultiplexProgramPacketIdentifiersMap
---
