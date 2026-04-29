---
description: The multiplex program object.
layout: schema
name: MultiplexProgram
properties_list:
- description: ''
  name: ChannelId
  type: object
- description: ''
  name: MultiplexProgramSettings
  type: object
- description: ''
  name: PacketIdentifiersMap
  type: object
- description: ''
  name: PipelineDetails
  type: object
- description: ''
  name: ProgramName
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-multiplex-program-schema.json
slug: medialive-api-multiplex-program
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-program-schema.json\",\n  \"title\": \"MultiplexProgram\",\n  \"description\": \"The multiplex program object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChannelId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelId\"\n          },\n          \"description\": \"The MediaLive channel associated with the program.\"\n        }\n      ]\n    },\n    \"MultiplexProgramSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiplexProgramSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"multiplexProgramSettings\"\n          },\n          \"description\": \"The settings for this multiplex program.\"\
  \n        }\n      ]\n    },\n    \"PacketIdentifiersMap\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiplexProgramPacketIdentifiersMap\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"packetIdentifiersMap\"\n          },\n          \"description\": \"The packet identifier map for this multiplex program.\"\n        }\n      ]\n    },\n    \"PipelineDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMultiplexProgramPipelineDetail\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pipelineDetails\"\n          },\n          \"description\": \"Contains information about the current sources for the specified program in the specified multiplex. Keep in mind that each multiplex pipeline connects to both pipelines in a given source channel (the channel identified by the program). But only one of those channel pipelines is ever active at one time.\"\n        }\n      ]\n\
  \    },\n    \"ProgramName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"programName\"\n          },\n          \"description\": \"The name of the multiplex program.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-program-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MultiplexProgram
---
