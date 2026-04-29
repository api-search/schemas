---
description: Live Event input parameters. There can be multiple inputs in a single Live Event.
layout: schema
name: InputSettings
properties_list:
- description: ''
  name: AudioSelectors
  type: object
- description: ''
  name: CaptionSelectors
  type: object
- description: ''
  name: DeblockFilter
  type: object
- description: ''
  name: DenoiseFilter
  type: object
- description: ''
  name: FilterStrength
  type: object
- description: ''
  name: InputFilter
  type: object
- description: ''
  name: NetworkInputSettings
  type: object
- description: ''
  name: Scte35Pid
  type: object
- description: ''
  name: Smpte2038DataPreference
  type: object
- description: ''
  name: SourceEndBehavior
  type: object
- description: ''
  name: VideoSelector
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-settings-schema.json
slug: medialive-api-input-settings
source_filename: medialive-api-input-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-settings-schema.json\",\n  \"title\": \"InputSettings\",\n  \"description\": \"Live Event input parameters. There can be multiple inputs in a single Live Event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioSelectors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAudioSelector\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioSelectors\"\n          },\n          \"description\": \"Used to select the audio stream to decode for inputs that have multiple available.\"\n        }\n      ]\n    },\n    \"CaptionSelectors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfCaptionSelector\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captionSelectors\"\
  \n          },\n          \"description\": \"Used to select the caption input to use for inputs that have multiple available.\"\n        }\n      ]\n    },\n    \"DeblockFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeblockFilter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deblockFilter\"\n          },\n          \"description\": \"Enable or disable the deblock filter when filtering.\"\n        }\n      ]\n    },\n    \"DenoiseFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDenoiseFilter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"denoiseFilter\"\n          },\n          \"description\": \"Enable or disable the denoise filter when filtering.\"\n        }\n      ]\n    },\n    \"FilterStrength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max5\"\n        },\n        {\n          \"xml\": {\n     \
  \       \"name\": \"filterStrength\"\n          },\n          \"description\": \"Adjusts the magnitude of filtering from 1 (minimal) to 5 (strongest).\"\n        }\n      ]\n    },\n    \"InputFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputFilter\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputFilter\"\n          },\n          \"description\": \"Turns on the filter for this input. MPEG-2 inputs have the deblocking filter enabled by default.\\n1) auto - filtering will be applied depending on input type/quality\\n2) disabled - no filtering will be applied to the input\\n3) forced - filtering will be applied regardless of input type\"\n        }\n      ]\n    },\n    \"NetworkInputSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkInputSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkInputSettings\"\n          },\n          \"description\"\
  : \"Input settings.\"\n        }\n      ]\n    },\n    \"Scte35Pid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8191\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35Pid\"\n          },\n          \"description\": \"PID from which to read SCTE-35 messages. If left undefined, EML will select the first SCTE-35 PID found in the input.\"\n        }\n      ]\n    },\n    \"Smpte2038DataPreference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Smpte2038DataPreference\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"smpte2038DataPreference\"\n          },\n          \"description\": \"Specifies whether to extract applicable ancillary data from a SMPTE-2038 source in this input. Applicable data types are captions, timecode, AFD, and SCTE-104 messages.\\n- PREFER: Extract from SMPTE-2038 if present in this input, otherwise extract from another source (if any).\\\
  n- IGNORE: Never extract any ancillary data from SMPTE-2038.\"\n        }\n      ]\n    },\n    \"SourceEndBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputSourceEndBehavior\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceEndBehavior\"\n          },\n          \"description\": \"Loop input if it is a file. This allows a file input to be streamed indefinitely.\"\n        }\n      ]\n    },\n    \"VideoSelector\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoSelector\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"videoSelector\"\n          },\n          \"description\": \"Informs which video elementary stream to decode for input types that have multiple available.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputSettings
---
