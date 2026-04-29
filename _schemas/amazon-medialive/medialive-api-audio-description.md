---
description: Audio Description
layout: schema
name: AudioDescription
properties_list:
- description: ''
  name: AudioNormalizationSettings
  type: object
- description: ''
  name: AudioSelectorName
  type: object
- description: ''
  name: AudioType
  type: object
- description: ''
  name: AudioTypeControl
  type: object
- description: ''
  name: AudioWatermarkingSettings
  type: object
- description: ''
  name: CodecSettings
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: LanguageCodeControl
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RemixSettings
  type: object
- description: ''
  name: StreamName
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-audio-description-schema.json
slug: medialive-api-audio-description
source_filename: medialive-api-audio-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-description-schema.json\",\n  \"title\": \"AudioDescription\",\n  \"description\": \"Audio Description\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioNormalizationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioNormalizationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioNormalizationSettings\"\n          },\n          \"description\": \"Advanced audio normalization settings.\"\n        }\n      ]\n    },\n    \"AudioSelectorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioSelectorName\"\n          },\n          \"description\": \"The name of the AudioSelector used\
  \ as the source for this AudioDescription.\"\n        }\n      ]\n    },\n    \"AudioType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioType\"\n          },\n          \"description\": \"Applies only if audioTypeControl is useConfigured. The values for audioType are defined in ISO-IEC 13818-1.\"\n        }\n      ]\n    },\n    \"AudioTypeControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioDescriptionAudioTypeControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioTypeControl\"\n          },\n          \"description\": \"Determines how audio type is determined.\\n  followInput: If the input contains an ISO 639 audioType, then that value is passed through to the output. If the input contains no ISO 639 audioType, the value in Audio Type is included in the output.\\n  useConfigured: The value in Audio\
  \ Type is included in the output.\\nNote that this field and audioType are both ignored if inputType is broadcasterMixedAd.\"\n        }\n      ]\n    },\n    \"AudioWatermarkingSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioWatermarkSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioWatermarkingSettings\"\n          },\n          \"description\": \"Settings to configure one or more solutions that insert audio watermarks in the audio encode\"\n        }\n      ]\n    },\n    \"CodecSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioCodecSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"codecSettings\"\n          },\n          \"description\": \"Audio codec settings.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max35\"\n        },\n     \
  \   {\n          \"xml\": {\n            \"name\": \"languageCode\"\n          },\n          \"description\": \"RFC 5646 language code representing the language of the audio output track. Only used if languageControlMode is useConfigured, or there is no ISO 639 language code specified in the input.\"\n        }\n      ]\n    },\n    \"LanguageCodeControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioDescriptionLanguageCodeControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"languageCodeControl\"\n          },\n          \"description\": \"Choosing followInput will cause the ISO 639 language code of the output to follow the ISO 639 language code of the input. The languageCode will be used when useConfigured is set, or when followInput is selected but there is no ISO 639 language code specified by the input.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMax255\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of this AudioDescription. Outputs will use this name to uniquely identify this AudioDescription.  Description names should be unique within this Live Event.\"\n        }\n      ]\n    },\n    \"RemixSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemixSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"remixSettings\"\n          },\n          \"description\": \"Settings that control how input audio channels are remixed into the output audio channels.\"\n        }\n      ]\n    },\n    \"StreamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"streamName\"\n          },\n          \"description\": \"Used for MS Smooth and Apple HLS outputs. Indicates the name displayed by the\
  \ player (eg. English, or Director Commentary).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AudioSelectorName\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-audio-description-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioDescription
---
