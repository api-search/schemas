---
description: Settings specific to Teletext caption sources, including Page number.
layout: schema
name: TeletextSourceSettings
properties_list:
- description: ''
  name: PageNumber
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-teletext-source-settings-schema.json
slug: mediaconvert-api-teletext-source-settings
source_filename: mediaconvert-api-teletext-source-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-teletext-source-settings-schema.json\",\n  \"title\": \"TeletextSourceSettings\",\n  \"description\": \"Settings specific to Teletext caption sources, including Page number.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PageNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin3Max3Pattern1809aFAF09aEAE\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pageNumber\"\n          },\n          \"description\": \"Use Page Number (PageNumber) to specify the three-digit hexadecimal page number that will be used for Teletext captions. Do not use this setting if you are passing through teletext from the input source to output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-teletext-source-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: TeletextSourceSettings
---
