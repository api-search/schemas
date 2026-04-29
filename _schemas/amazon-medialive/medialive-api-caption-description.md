---
description: Caption Description
layout: schema
name: CaptionDescription
properties_list:
- description: ''
  name: Accessibility
  type: object
- description: ''
  name: CaptionSelectorName
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
- description: ''
  name: Name
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-caption-description-schema.json
slug: medialive-api-caption-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-caption-description-schema.json\",\n  \"title\": \"CaptionDescription\",\n  \"description\": \"Caption Description\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Accessibility\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessibilityType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accessibility\"\n          },\n          \"description\": \"Indicates whether the caption track implements accessibility features such as written descriptions of spoken dialog, music, and sounds.\"\n        }\n      ]\n    },\n    \"CaptionSelectorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"captionSelectorName\"\n     \
  \     },\n          \"description\": \"Specifies which input caption selector to use as a caption source when generating output captions. This field should match a captionSelector name.\"\n        }\n      ]\n    },\n    \"DestinationSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CaptionDestinationSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationSettings\"\n          },\n          \"description\": \"Additional settings for captions destination that depend on the destination type.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"languageCode\"\n          },\n          \"description\": \"ISO 639-2 three-digit code: http://www.loc.gov/standards/iso639-2/\"\n        }\n      ]\n    },\n    \"LanguageDescription\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"languageDescription\"\n          },\n          \"description\": \"Human readable information to indicate captions available for players (eg. English, or Spanish).\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Name of the caption description.  Used to associate a caption description with an output.  Names must be unique within an event.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CaptionSelectorName\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-caption-description-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CaptionDescription
---
