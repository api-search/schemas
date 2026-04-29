---
description: Maps a caption channel to an ISO 693-2 language code (http://www.loc.gov/standards/iso639-2), with an optional description.
layout: schema
name: CaptionLanguageMapping
properties_list:
- description: ''
  name: CaptionChannel
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: LanguageDescription
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-caption-language-mapping-schema.json
slug: medialive-api-caption-language-mapping
source_filename: medialive-api-caption-language-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-caption-language-mapping-schema.json\",\n  \"title\": \"CaptionLanguageMapping\",\n  \"description\": \"Maps a caption channel to an ISO 693-2 language code (http://www.loc.gov/standards/iso639-2), with an optional description.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CaptionChannel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max4\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captionChannel\"\n          },\n          \"description\": \"The closed caption channel being described by this CaptionLanguageMapping.  Each channel mapping must have a unique channel number (maximum of 4)\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin3Max3\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"languageCode\"\n          },\n          \"description\": \"Three character ISO 639-2 language code (see http://www.loc.gov/standards/iso639-2)\"\n        }\n      ]\n    },\n    \"LanguageDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"languageDescription\"\n          },\n          \"description\": \"Textual description of language\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LanguageCode\",\n    \"LanguageDescription\",\n    \"CaptionChannel\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-caption-language-mapping-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CaptionLanguageMapping
---
