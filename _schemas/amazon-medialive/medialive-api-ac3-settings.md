---
description: Ac3 Settings
layout: schema
name: Ac3Settings
properties_list:
- description: ''
  name: Bitrate
  type: object
- description: ''
  name: BitstreamMode
  type: object
- description: ''
  name: CodingMode
  type: object
- description: ''
  name: Dialnorm
  type: object
- description: ''
  name: DrcProfile
  type: object
- description: ''
  name: LfeFilter
  type: object
- description: ''
  name: MetadataControl
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-ac3-settings-schema.json
slug: medialive-api-ac3-settings
source_filename: medialive-api-ac3-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-ac3-settings-schema.json\",\n  \"title\": \"Ac3Settings\",\n  \"description\": \"Ac3 Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"Average bitrate in bits/second. Valid bitrates depend on the coding mode.\"\n        }\n      ]\n    },\n    \"BitstreamMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ac3BitstreamMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitstreamMode\"\n          },\n          \"description\": \"Specifies the bitstream mode (bsmod) for the emitted AC-3 stream. See ATSC\
  \ A/52-2012 for background on these values.\"\n        }\n      ]\n    },\n    \"CodingMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ac3CodingMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codingMode\"\n          },\n          \"description\": \"Dolby Digital coding mode. Determines number of channels.\"\n        }\n      ]\n    },\n    \"Dialnorm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max31\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dialnorm\"\n          },\n          \"description\": \"Sets the dialnorm for the output. If excluded and input audio is Dolby Digital, dialnorm will be passed through.\"\n        }\n      ]\n    },\n    \"DrcProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ac3DrcProfile\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"drcProfile\"\n          },\n\
  \          \"description\": \"If set to filmStandard, adds dynamic range compression signaling to the output bitstream as defined in the Dolby Digital specification.\"\n        }\n      ]\n    },\n    \"LfeFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ac3LfeFilter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lfeFilter\"\n          },\n          \"description\": \"When set to enabled, applies a 120Hz lowpass filter to the LFE channel prior to encoding. Only valid in codingMode32Lfe mode.\"\n        }\n      ]\n    },\n    \"MetadataControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ac3MetadataControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"metadataControl\"\n          },\n          \"description\": \"When set to \\\"followInput\\\", encoder metadata will be sourced from the DD, DD+, or DolbyE decoder that supplied this audio data. If audio was not supplied\
  \ from one of these streams, then the static metadata settings will be used.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-ac3-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Ac3Settings
---
