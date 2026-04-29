---
description: Use audio selector groups to combine multiple sidecar audio inputs so that you can assign them to a single output audio tab (AudioDescription). Note that, if you're working with embedded audio, it's simpler to assign multiple input tracks into a single audio selector rather than use an audio selector group.
layout: schema
name: AudioSelectorGroup
properties_list:
- description: ''
  name: AudioSelectorNames
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-audio-selector-group-schema.json
slug: mediaconvert-api-audio-selector-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-selector-group-schema.json\",\n  \"title\": \"AudioSelectorGroup\",\n  \"description\": \"Use audio selector groups to combine multiple sidecar audio inputs so that you can assign them to a single output audio tab (AudioDescription). Note that, if you're working with embedded audio, it's simpler to assign multiple input tracks into a single audio selector rather than use an audio selector group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioSelectorNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__stringMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audioSelectorNames\"\n          },\n          \"description\": \"Name of an Audio Selector within the same input to include in the group. Audio\
  \ selector names are standardized, based on their order within the input (e.g., \\\"Audio Selector 1\\\"). The audio selector name parameter can be repeated to add any number of audio selectors to the group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-selector-group-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioSelectorGroup
---
