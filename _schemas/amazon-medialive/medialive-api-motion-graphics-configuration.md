---
description: Motion Graphics Configuration
layout: schema
name: MotionGraphicsConfiguration
properties_list:
- description: ''
  name: MotionGraphicsInsertion
  type: object
- description: ''
  name: MotionGraphicsSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-motion-graphics-configuration-schema.json
slug: medialive-api-motion-graphics-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-motion-graphics-configuration-schema.json\",\n  \"title\": \"MotionGraphicsConfiguration\",\n  \"description\": \"Motion Graphics Configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MotionGraphicsInsertion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MotionGraphicsInsertion\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"motionGraphicsInsertion\"\n          }\n        }\n      ]\n    },\n    \"MotionGraphicsSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MotionGraphicsSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"motionGraphicsSettings\"\n          },\n          \"description\": \"Motion Graphics Settings\"\n        }\n      ]\n    }\n \
  \ },\n  \"required\": [\n    \"MotionGraphicsSettings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-motion-graphics-configuration-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MotionGraphicsConfiguration
---
