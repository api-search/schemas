---
description: Specify which source for language code takes precedence for this audio track. When you choose Follow input (FOLLOW_INPUT), the service uses the language code from the input track if it's present. If there's no languge code on the input track, the service uses the code that you specify in the setting Language code (languageCode or customLanguageCode). When you choose Use configured (USE_CONFIGURED), the service uses the language code that you specify.
layout: schema
name: AudioLanguageCodeControl
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-audio-language-code-control-schema.json
slug: mediaconvert-api-audio-language-code-control
source_filename: mediaconvert-api-audio-language-code-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-language-code-control-schema.json\",\n  \"title\": \"AudioLanguageCodeControl\",\n  \"description\": \"Specify which source for language code takes precedence for this audio track. When you choose Follow input (FOLLOW_INPUT), the service uses the language code from the input track if it's present. If there's no languge code on the input track, the service uses the code that you specify in the setting Language code (languageCode or customLanguageCode). When you choose Use configured (USE_CONFIGURED), the service uses the language code that you specify.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"FOLLOW_INPUT\",\n    \"USE_CONFIGURED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-audio-language-code-control-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AudioLanguageCodeControl
---
