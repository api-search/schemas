---
description: Enable this setting on one audio selector to set it as the default for the job. The service uses this default for outputs where it can't find the specified input audio. If you don't set a default, those outputs have no audio.
layout: schema
name: AudioDefaultSelection
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-audio-default-selection-schema.json
slug: mediaconvert-api-audio-default-selection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-default-selection-schema.json\",\n  \"title\": \"AudioDefaultSelection\",\n  \"description\": \"Enable this setting on one audio selector to set it as the default for the job. The service uses this default for outputs where it can't find the specified input audio. If you don't set a default, those outputs have no audio.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"DEFAULT\",\n    \"NOT_DEFAULT\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-default-selection-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioDefaultSelection
---
