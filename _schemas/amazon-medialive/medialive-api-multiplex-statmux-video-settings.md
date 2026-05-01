---
description: Statmux rate control settings
layout: schema
name: MultiplexStatmuxVideoSettings
properties_list:
- description: ''
  name: MaximumBitrate
  type: object
- description: ''
  name: MinimumBitrate
  type: object
- description: ''
  name: Priority
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-multiplex-statmux-video-settings-schema.json
slug: medialive-api-multiplex-statmux-video-settings
source_filename: medialive-api-multiplex-statmux-video-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-statmux-video-settings-schema.json\",\n  \"title\": \"MultiplexStatmuxVideoSettings\",\n  \"description\": \"Statmux rate control settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaximumBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin100000Max100000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maximumBitrate\"\n          },\n          \"description\": \"Maximum statmux bitrate.\"\n        }\n      ]\n    },\n    \"MinimumBitrate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin100000Max100000000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minimumBitrate\"\n          },\n          \"description\": \"Minimum statmux\
  \ bitrate.\"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative5Max5\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"priority\"\n          },\n          \"description\": \"The purpose of the priority is to use a combination of the\\\\nmultiplex rate control algorithm and the QVBR capability of the\\\\nencoder to prioritize the video quality of some channels in a\\\\nmultiplex over others.  Channels that have a higher priority will\\\\nget higher video quality at the expense of the video quality of\\\\nother channels in the multiplex with lower priority.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-multiplex-statmux-video-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: MultiplexStatmuxVideoSettings
---
