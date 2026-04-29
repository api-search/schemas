---
description: OutputChannel mapping settings.
layout: schema
name: OutputChannelMapping
properties_list:
- description: ''
  name: InputChannels
  type: object
- description: ''
  name: InputChannelsFineTune
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-output-channel-mapping-schema.json
slug: mediaconvert-api-output-channel-mapping
source_filename: mediaconvert-api-output-channel-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-channel-mapping-schema.json\",\n  \"title\": \"OutputChannelMapping\",\n  \"description\": \"OutputChannel mapping settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputChannels\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__integerMinNegative60Max6\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputChannels\"\n          },\n          \"description\": \"Use this setting to specify your remix values when they are integers, such as -10, 0, or 4.\"\n        }\n      ]\n    },\n    \"InputChannelsFineTune\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__doubleMinNegative60Max6\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputChannelsFineTune\"\
  \n          },\n          \"description\": \"Use this setting to specify your remix values when they have a decimal component, such as -10.312, 0.08, or 4.9. MediaConvert rounds your remixing values to the nearest thousandth.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-output-channel-mapping-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: OutputChannelMapping
---
