---
description: Container specific settings.
layout: schema
name: ContainerSettings
properties_list:
- description: ''
  name: CmfcSettings
  type: object
- description: ''
  name: Container
  type: object
- description: ''
  name: F4vSettings
  type: object
- description: ''
  name: M2tsSettings
  type: object
- description: ''
  name: M3u8Settings
  type: object
- description: ''
  name: MovSettings
  type: object
- description: ''
  name: Mp4Settings
  type: object
- description: ''
  name: MpdSettings
  type: object
- description: ''
  name: MxfSettings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-container-settings-schema.json
slug: mediaconvert-api-container-settings
source_filename: mediaconvert-api-container-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-container-settings-schema.json\",\n  \"title\": \"ContainerSettings\",\n  \"description\": \"Container specific settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CmfcSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CmfcSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cmfcSettings\"\n          },\n          \"description\": \"These settings relate to the fragmented MP4 container for the segments in your CMAF outputs.\"\n        }\n      ]\n    },\n    \"Container\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"container\"\n          },\n          \"description\": \"Container for this\
  \ output. Some containers require a container settings object. If not specified, the default object will be created.\"\n        }\n      ]\n    },\n    \"F4vSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/F4vSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"f4vSettings\"\n          },\n          \"description\": \"Settings for F4v container\"\n        }\n      ]\n    },\n    \"M2tsSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M2tsSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"m2tsSettings\"\n          },\n          \"description\": \"MPEG-2 TS container settings. These apply to outputs in a File output group when the output's container (ContainerType) is MPEG-2 Transport Stream (M2TS). In these assets, data is organized by the program map table (PMT). Each transport stream program contains subsets of data, including audio, video, and metadata.\
  \ Each of these subsets of data has a numerical label called a packet identifier (PID). Each transport stream program corresponds to one MediaConvert output. The PMT lists the types of data in a program along with their PID. Downstream systems and players use the program map table to look up the PID for each type of data it accesses and then uses the PIDs to locate specific data within the asset.\"\n        }\n      ]\n    },\n    \"M3u8Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/M3u8Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"m3u8Settings\"\n          },\n          \"description\": \"These settings relate to the MPEG-2 transport stream (MPEG2-TS) container for the MPEG2-TS segments in your HLS outputs.\"\n        }\n      ]\n    },\n    \"MovSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MovSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"movSettings\"\n          },\n          \"description\": \"These settings relate to your QuickTime MOV output container.\"\n        }\n      ]\n    },\n    \"Mp4Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Mp4Settings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mp4Settings\"\n          },\n          \"description\": \"These settings relate to your MP4 output container. You can create audio only outputs with this container. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/supported-codecs-containers-audio-only.html#output-codecs-and-containers-supported-for-audio-only.\"\n        }\n      ]\n    },\n    \"MpdSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MpdSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mpdSettings\"\n          },\n          \"description\": \"These settings relate to the fragmented MP4 container\
  \ for the segments in your DASH outputs.\"\n        }\n      ]\n    },\n    \"MxfSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MxfSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mxfSettings\"\n          },\n          \"description\": \"These settings relate to your MXF output container.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-container-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ContainerSettings
---
