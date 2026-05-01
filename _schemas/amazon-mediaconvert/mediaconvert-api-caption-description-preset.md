---
description: Caption Description for preset
layout: schema
name: CaptionDescriptionPreset
properties_list:
- description: ''
  name: CustomLanguageCode
  type: object
- description: ''
  name: DestinationSettings
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: LanguageDescription
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-caption-description-preset-schema.json
slug: mediaconvert-api-caption-description-preset
source_filename: mediaconvert-api-caption-description-preset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-caption-description-preset-schema.json\",\n  \"title\": \"CaptionDescriptionPreset\",\n  \"description\": \"Caption Description for preset\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CustomLanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternAZaZ23AZaZ\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"customLanguageCode\"\n          },\n          \"description\": \"Specify the language for this captions output track. For most captions output formats, the encoder puts this language information in the output captions metadata. If your output captions format is DVB-Sub or Burn in, the encoder uses this language information when automatically selecting the font script for rendering the captions text.\
  \ For all outputs, you can use an ISO 639-2 or ISO 639-3 code. For streaming outputs, you can also use any other code in the full RFC-5646 specification. Streaming outputs are those that are in one of the following output groups: CMAF, DASH ISO, Apple HLS, or Microsoft Smooth Streaming.\"\n        }\n      ]\n    },\n    \"DestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CaptionDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationSettings\"\n          },\n          \"description\": \"Settings related to one captions tab on the MediaConvert console. In your job JSON, an instance of captions DestinationSettings is equivalent to one captions tab in the console. Usually, one captions tab corresponds to one output captions track. Depending on your output captions format, one tab might correspond to a set of output captions tracks. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/including-captions.html.\"\
  \n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"languageCode\"\n          },\n          \"description\": \"Specify the language of this captions output track. For most captions output formats, the encoder puts this language information in the output captions metadata. If your output captions format is DVB-Sub or Burn in, the encoder uses this language information to choose the font language for rendering the captions text.\"\n        }\n      ]\n    },\n    \"LanguageDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"languageDescription\"\n          },\n          \"description\": \"Specify a label for this set of output captions. For example, \\\"English\\\", \\\"Director commentary\\\", or \\\"track_2\\\
  \". For streaming outputs, MediaConvert passes this information into destination manifests for display on the end-viewer's player device. For outputs in other output groups, the service ignores this setting.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-caption-description-preset-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CaptionDescriptionPreset
---
