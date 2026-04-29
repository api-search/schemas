---
description: The video configuration for each program in a multiplex.
layout: schema
name: MultiplexVideoSettings
properties_list:
- description: ''
  name: ConstantBitrate
  type: object
- description: ''
  name: StatmuxSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-multiplex-video-settings-schema.json
slug: medialive-api-multiplex-video-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-video-settings-schema.json\",\n  \"title\": \"MultiplexVideoSettings\",\n  \"description\": \"The video configuration for each program in a multiplex.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConstantBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin100000Max100000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"constantBitrate\"\n          },\n          \"description\": \"The constant bitrate configuration for the video encode.\\nWhen this field is defined, StatmuxSettings must be undefined.\"\n        }\n      ]\n    },\n    \"StatmuxSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiplexStatmuxVideoSettings\"\n        },\n        {\n        \
  \  \"xml\": {\n            \"name\": \"statmuxSettings\"\n          },\n          \"description\": \"Statmux rate control settings.\\nWhen this field is defined, ConstantBitrate must be undefined.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-video-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MultiplexVideoSettings
---
