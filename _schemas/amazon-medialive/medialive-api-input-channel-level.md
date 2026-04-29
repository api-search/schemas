---
description: Input Channel Level
layout: schema
name: InputChannelLevel
properties_list:
- description: ''
  name: Gain
  type: object
- description: ''
  name: InputChannel
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-channel-level-schema.json
slug: medialive-api-input-channel-level
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-channel-level-schema.json\",\n  \"title\": \"InputChannelLevel\",\n  \"description\": \"Input Channel Level\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Gain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative60Max6\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"gain\"\n          },\n          \"description\": \"Remixing value. Units are in dB and acceptable values are within the range from -60 (mute) and 6 dB.\"\n        }\n      ]\n    },\n    \"InputChannel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max15\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputChannel\"\n          },\n          \"description\": \"The index of\
  \ the input channel used as a source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InputChannel\",\n    \"Gain\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-channel-level-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: InputChannelLevel
---
