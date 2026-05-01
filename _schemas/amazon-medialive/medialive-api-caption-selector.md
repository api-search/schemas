---
description: Caption Selector
layout: schema
name: CaptionSelector
properties_list:
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: SelectorSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-caption-selector-schema.json
slug: medialive-api-caption-selector
source_filename: medialive-api-caption-selector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-caption-selector-schema.json\",\n  \"title\": \"CaptionSelector\",\n  \"description\": \"Caption Selector\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"languageCode\"\n          },\n          \"description\": \"When specified this field indicates the three letter language code of the caption track to extract from the source.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Name identifier for a caption\
  \ selector.  This name is used to associate this caption selector with one or more caption descriptions.  Names must be unique within an event.\"\n        }\n      ]\n    },\n    \"SelectorSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CaptionSelectorSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"selectorSettings\"\n          },\n          \"description\": \"Caption selector settings.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-caption-selector-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CaptionSelector
---
