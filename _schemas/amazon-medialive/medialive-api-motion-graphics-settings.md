---
description: Motion Graphics Settings
layout: schema
name: MotionGraphicsSettings
properties_list:
- description: ''
  name: HtmlMotionGraphicsSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-motion-graphics-settings-schema.json
slug: medialive-api-motion-graphics-settings
source_filename: medialive-api-motion-graphics-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-motion-graphics-settings-schema.json\",\n  \"title\": \"MotionGraphicsSettings\",\n  \"description\": \"Motion Graphics Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HtmlMotionGraphicsSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HtmlMotionGraphicsSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"htmlMotionGraphicsSettings\"\n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-motion-graphics-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MotionGraphicsSettings
---
