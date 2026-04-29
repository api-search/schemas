---
description: Eac3 Settings
layout: schema
name: Eac3Settings
properties_list:
- description: ''
  name: AttenuationControl
  type: object
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
  name: DcFilter
  type: object
- description: ''
  name: Dialnorm
  type: object
- description: ''
  name: DrcLine
  type: object
- description: ''
  name: DrcRf
  type: object
- description: ''
  name: LfeControl
  type: object
- description: ''
  name: LfeFilter
  type: object
- description: ''
  name: LoRoCenterMixLevel
  type: object
- description: ''
  name: LoRoSurroundMixLevel
  type: object
- description: ''
  name: LtRtCenterMixLevel
  type: object
- description: ''
  name: LtRtSurroundMixLevel
  type: object
- description: ''
  name: MetadataControl
  type: object
- description: ''
  name: PassthroughControl
  type: object
- description: ''
  name: PhaseControl
  type: object
- description: ''
  name: StereoDownmix
  type: object
- description: ''
  name: SurroundExMode
  type: object
- description: ''
  name: SurroundMode
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-eac3-settings-schema.json
slug: medialive-api-eac3-settings
source_filename: medialive-api-eac3-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-eac3-settings-schema.json\",\n  \"title\": \"Eac3Settings\",\n  \"description\": \"Eac3 Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AttenuationControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3AttenuationControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"attenuationControl\"\n          },\n          \"description\": \"When set to attenuate3Db, applies a 3 dB attenuation to the surround channels. Only used for 3/2 coding mode.\"\n        }\n      ]\n    },\n    \"Bitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitrate\"\n          },\n          \"description\": \"Average bitrate\
  \ in bits/second. Valid bitrates depend on the coding mode.\"\n        }\n      ]\n    },\n    \"BitstreamMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3BitstreamMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bitstreamMode\"\n          },\n          \"description\": \"Specifies the bitstream mode (bsmod) for the emitted E-AC-3 stream. See ATSC A/52-2012 (Annex E) for background on these values.\"\n        }\n      ]\n    },\n    \"CodingMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3CodingMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codingMode\"\n          },\n          \"description\": \"Dolby Digital Plus coding mode. Determines number of channels.\"\n        }\n      ]\n    },\n    \"DcFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3DcFilter\"\n        },\n        {\n          \"xml\": {\n       \
  \     \"name\": \"dcFilter\"\n          },\n          \"description\": \"When set to enabled, activates a DC highpass filter for all input channels.\"\n        }\n      ]\n    },\n    \"Dialnorm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max31\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dialnorm\"\n          },\n          \"description\": \"Sets the dialnorm for the output. If blank and input audio is Dolby Digital Plus, dialnorm will be passed through.\"\n        }\n      ]\n    },\n    \"DrcLine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3DrcLine\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"drcLine\"\n          },\n          \"description\": \"Sets the Dolby dynamic range compression profile.\"\n        }\n      ]\n    },\n    \"DrcRf\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3DrcRf\"\n        },\n  \
  \      {\n          \"xml\": {\n            \"name\": \"drcRf\"\n          },\n          \"description\": \"Sets the profile for heavy Dolby dynamic range compression, ensures that the instantaneous signal peaks do not exceed specified levels.\"\n        }\n      ]\n    },\n    \"LfeControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3LfeControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lfeControl\"\n          },\n          \"description\": \"When encoding 3/2 audio, setting to lfe enables the LFE channel\"\n        }\n      ]\n    },\n    \"LfeFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3LfeFilter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lfeFilter\"\n          },\n          \"description\": \"When set to enabled, applies a 120Hz lowpass filter to the LFE channel prior to encoding. Only valid with codingMode32 coding mode.\"\n        }\n    \
  \  ]\n    },\n    \"LoRoCenterMixLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"loRoCenterMixLevel\"\n          },\n          \"description\": \"Left only/Right only center mix level. Only used for 3/2 coding mode.\"\n        }\n      ]\n    },\n    \"LoRoSurroundMixLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"loRoSurroundMixLevel\"\n          },\n          \"description\": \"Left only/Right only surround mix level. Only used for 3/2 coding mode.\"\n        }\n      ]\n    },\n    \"LtRtCenterMixLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ltRtCenterMixLevel\"\n          },\n          \"description\": \"Left total/Right total center\
  \ mix level. Only used for 3/2 coding mode.\"\n        }\n      ]\n    },\n    \"LtRtSurroundMixLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ltRtSurroundMixLevel\"\n          },\n          \"description\": \"Left total/Right total surround mix level. Only used for 3/2 coding mode.\"\n        }\n      ]\n    },\n    \"MetadataControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3MetadataControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"metadataControl\"\n          },\n          \"description\": \"When set to followInput, encoder metadata will be sourced from the DD, DD+, or DolbyE decoder that supplied this audio data. If audio was not supplied from one of these streams, then the static metadata settings will be used.\"\n        }\n      ]\n    },\n    \"PassthroughControl\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/Eac3PassthroughControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"passthroughControl\"\n          },\n          \"description\": \"When set to whenPossible, input DD+ audio will be passed through if it is present on the input. This detection is dynamic over the life of the transcode. Inputs that alternate between DD+ and non-DD+ content will have a consistent DD+ output as the system alternates between passthrough and encoding.\"\n        }\n      ]\n    },\n    \"PhaseControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3PhaseControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"phaseControl\"\n          },\n          \"description\": \"When set to shift90Degrees, applies a 90-degree phase shift to the surround channels. Only used for 3/2 coding mode.\"\n        }\n      ]\n    },\n    \"StereoDownmix\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/Eac3StereoDownmix\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"stereoDownmix\"\n          },\n          \"description\": \"Stereo downmix preference. Only used for 3/2 coding mode.\"\n        }\n      ]\n    },\n    \"SurroundExMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3SurroundExMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"surroundExMode\"\n          },\n          \"description\": \"When encoding 3/2 audio, sets whether an extra center back surround channel is matrix encoded into the left and right surround channels.\"\n        }\n      ]\n    },\n    \"SurroundMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eac3SurroundMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"surroundMode\"\n          },\n          \"description\": \"When encoding 2/0 audio, sets whether Dolby Surround\
  \ is matrix encoded into the two channels.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-eac3-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Eac3Settings
---
