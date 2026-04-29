---
description: Aac Settings
layout: schema
name: AacSettings
properties_list:
- description: ''
  name: Bitrate
  type: object
- description: ''
  name: CodingMode
  type: object
- description: ''
  name: InputType
  type: object
- description: ''
  name: Profile
  type: object
- description: ''
  name: RateControlMode
  type: object
- description: ''
  name: RawFormat
  type: object
- description: ''
  name: SampleRate
  type: object
- description: ''
  name: Spec
  type: object
- description: ''
  name: VbrQuality
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-aac-settings-schema.json
slug: medialive-api-aac-settings
source_filename: medialive-api-aac-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-aac-settings-schema.json\",\n  \"title\": \"AacSettings\",\n  \"description\": \"Aac Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"Average bitrate in bits/second. Valid values depend on rate control mode and profile.\"\n        }\n      ]\n    },\n    \"CodingMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AacCodingMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codingMode\"\n          },\n          \"description\": \"Mono, Stereo, or 5.1 channel layout. Valid values depend on rate control\
  \ mode and profile. The adReceiverMix setting receives a stereo description plus control track and emits a mono AAC encode of the description track, with control data emitted in the PES header as per ETSI TS 101 154 Annex E.\"\n        }\n      ]\n    },\n    \"InputType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AacInputType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputType\"\n          },\n          \"description\": \"Set to \\\"broadcasterMixedAd\\\" when input contains pre-mixed main audio + AD (narration) as a stereo pair.  The Audio Type field (audioType) will be set to 3, which signals to downstream systems that this stream contains \\\"broadcaster mixed AD\\\". Note that the input received by the encoder must contain pre-mixed audio; the encoder does not perform the mixing. The values in audioTypeControl and audioType (in AudioDescription) are ignored when set to broadcasterMixedAd.\\n\\nLeave set to \\\"normal\\\
  \" when input does not contain pre-mixed audio + AD.\"\n        }\n      ]\n    },\n    \"Profile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AacProfile\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"profile\"\n          },\n          \"description\": \"AAC Profile.\"\n        }\n      ]\n    },\n    \"RateControlMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AacRateControlMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rateControlMode\"\n          },\n          \"description\": \"Rate Control Mode.\"\n        }\n      ]\n    },\n    \"RawFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AacRawFormat\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rawFormat\"\n          },\n          \"description\": \"Sets LATM / LOAS AAC output for raw containers.\"\n        }\n      ]\n    },\n    \"SampleRate\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sampleRate\"\n          },\n          \"description\": \"Sample rate in Hz. Valid values depend on rate control mode and profile.\"\n        }\n      ]\n    },\n    \"Spec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AacSpec\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"spec\"\n          },\n          \"description\": \"Use MPEG-2 AAC audio instead of MPEG-4 AAC audio for raw or MPEG-2 Transport Stream containers.\"\n        }\n      ]\n    },\n    \"VbrQuality\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AacVbrQuality\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vbrQuality\"\n          },\n          \"description\": \"VBR Quality Level - Only used if rateControlMode is VBR.\"\n        }\n      ]\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-aac-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AacSettings
---
