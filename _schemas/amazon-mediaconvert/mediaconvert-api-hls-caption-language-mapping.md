---
description: Caption Language Mapping
layout: schema
name: HlsCaptionLanguageMapping
properties_list:
- description: ''
  name: CaptionChannel
  type: object
- description: ''
  name: CustomLanguageCode
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: LanguageDescription
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-caption-language-mapping-schema.json
slug: mediaconvert-api-hls-caption-language-mapping
source_filename: mediaconvert-api-hls-caption-language-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-caption-language-mapping-schema.json\",\n  \"title\": \"HlsCaptionLanguageMapping\",\n  \"description\": \"Caption Language Mapping\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CaptionChannel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative2147483648Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captionChannel\"\n          },\n          \"description\": \"Caption channel.\"\n        }\n      ]\n    },\n    \"CustomLanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin3Max3PatternAZaZ3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"customLanguageCode\"\n          },\n          \"description\": \"Specify the\
  \ language for this captions channel, using the ISO 639-2 or ISO 639-3 three-letter language code\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"languageCode\"\n          },\n          \"description\": \"Specify the language, using the ISO 639-2 three-letter code listed at https://www.loc.gov/standards/iso639-2/php/code_list.php.\"\n        }\n      ]\n    },\n    \"LanguageDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"languageDescription\"\n          },\n          \"description\": \"Caption language description.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-caption-language-mapping-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsCaptionLanguageMapping
---
