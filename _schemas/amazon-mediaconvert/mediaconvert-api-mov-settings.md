---
description: These settings relate to your QuickTime MOV output container.
layout: schema
name: MovSettings
properties_list:
- description: ''
  name: ClapAtom
  type: object
- description: ''
  name: CslgAtom
  type: object
- description: ''
  name: Mpeg2FourCCControl
  type: object
- description: ''
  name: PaddingControl
  type: object
- description: ''
  name: Reference
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-mov-settings-schema.json
slug: mediaconvert-api-mov-settings
source_filename: mediaconvert-api-mov-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mov-settings-schema.json\",\n  \"title\": \"MovSettings\",\n  \"description\": \"These settings relate to your QuickTime MOV output container.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClapAtom\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MovClapAtom\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clapAtom\"\n          },\n          \"description\": \"When enabled, include 'clap' atom if appropriate for the video output settings.\"\n        }\n      ]\n    },\n    \"CslgAtom\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MovCslgAtom\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cslgAtom\"\n          },\n          \"description\": \"When enabled, file composition\
  \ times will start at zero, composition times in the 'ctts' (composition time to sample) box for B-frames will be negative, and a 'cslg' (composition shift least greatest) box will be included per 14496-1 amendment 1. This improves compatibility with Apple players and tools.\"\n        }\n      ]\n    },\n    \"Mpeg2FourCCControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MovMpeg2FourCCControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mpeg2FourCCControl\"\n          },\n          \"description\": \"When set to XDCAM, writes MPEG2 video streams into the QuickTime file using XDCAM fourcc codes. This increases compatibility with Apple editors and players, but may decrease compatibility with other players. Only applicable when the video codec is MPEG2.\"\n        }\n      ]\n    },\n    \"PaddingControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MovPaddingControl\"\n        },\n        {\n\
  \          \"xml\": {\n            \"name\": \"paddingControl\"\n          },\n          \"description\": \"Unless you need Omneon compatibility: Keep the default value, None. To make this output compatible with Omneon: Choose Omneon. When you do, MediaConvert increases the length of the 'elst' edit list atom. Note that this might cause file rejections when a recipient of the output file doesn't expect this extra padding.\"\n        }\n      ]\n    },\n    \"Reference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MovReference\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"reference\"\n          },\n          \"description\": \"Always keep the default value (SELF_CONTAINED) for this setting.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mov-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MovSettings
---
