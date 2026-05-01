---
description: Use automated encoding to have MediaConvert choose your encoding settings for you, based on characteristics of your input video.
layout: schema
name: AutomatedEncodingSettings
properties_list:
- description: ''
  name: AbrSettings
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-automated-encoding-settings-schema.json
slug: mediaconvert-api-automated-encoding-settings
source_filename: mediaconvert-api-automated-encoding-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-automated-encoding-settings-schema.json\",\n  \"title\": \"AutomatedEncodingSettings\",\n  \"description\": \"Use automated encoding to have MediaConvert choose your encoding settings for you, based on characteristics of your input video.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AbrSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutomatedAbrSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"abrSettings\"\n          },\n          \"description\": \"Use automated ABR to have MediaConvert set up the renditions in your ABR package for you automatically, based on characteristics of your input video. This feature optimizes video quality while minimizing the overall size of your ABR package.\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-automated-encoding-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: AutomatedEncodingSettings
---
