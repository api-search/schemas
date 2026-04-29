---
description: Use captions selectors to specify the captions data from your input that you use in your outputs. You can use up to 20 captions selectors per input.
layout: schema
name: CaptionSelector
properties_list:
- description: ''
  name: CustomLanguageCode
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: SourceSettings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-caption-selector-schema.json
slug: mediaconvert-api-caption-selector
source_filename: mediaconvert-api-caption-selector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-caption-selector-schema.json\",\n  \"title\": \"CaptionSelector\",\n  \"description\": \"Use captions selectors to specify the captions data from your input that you use in your outputs. You can use up to 20 captions selectors per input.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CustomLanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin3Max3PatternAZaZ3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"customLanguageCode\"\n          },\n          \"description\": \"The specific language to extract from source, using the ISO 639-2 or ISO 639-3 three-letter language code. If input is SCTE-27, complete this field and/or PID to select the caption language to extract. If input is DVB-Sub and output\
  \ is Burn-in or SMPTE-TT, complete this field and/or PID to select the caption language to extract. If input is DVB-Sub that is being passed through, omit this field (and PID field); there is no way to extract a specific language with pass-through captions.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"languageCode\"\n          },\n          \"description\": \"The specific language to extract from source. If input is SCTE-27, complete this field and/or PID to select the caption language to extract. If input is DVB-Sub and output is Burn-in or SMPTE-TT, complete this field and/or PID to select the caption language to extract. If input is DVB-Sub that is being passed through, omit this field (and PID field); there is no way to extract a specific language with pass-through captions.\"\n        }\n      ]\n    },\n    \"SourceSettings\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CaptionSourceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceSettings\"\n          },\n          \"description\": \"If your input captions are SCC, TTML, STL, SMI, SRT, or IMSC in an xml file, specify the URI of the input captions source file. If your input captions are IMSC in an IMF package, use TrackSourceSettings instead of FileSoureSettings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-caption-selector-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CaptionSelector
---
