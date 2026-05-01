---
description: 'Set Accessibility subtitles to Enabled if the ISMC or WebVTT captions track is intended to provide accessibility for people who are deaf or hard of hearing. When you enable this feature, MediaConvert adds the following attributes under EXT-X-MEDIA in the HLS or CMAF manifest for this track: CHARACTERISTICS="public.accessibility.describes-spoken-dialog,public.accessibility.describes-music-and-sound" and AUTOSELECT="YES". Keep the default value, Disabled, if the captions track is not intended to provide such accessibility. MediaConvert will not add the above attributes.'
layout: schema
name: WebvttAccessibilitySubs
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-webvtt-accessibility-subs-schema.json
slug: mediaconvert-api-webvtt-accessibility-subs
source_filename: mediaconvert-api-webvtt-accessibility-subs-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-webvtt-accessibility-subs-schema.json\",\n  \"title\": \"WebvttAccessibilitySubs\",\n  \"description\": \"Set Accessibility subtitles to Enabled if the ISMC or WebVTT captions track is intended to provide accessibility for people who are deaf or hard of hearing. When you enable this feature, MediaConvert adds the following attributes under EXT-X-MEDIA in the HLS or CMAF manifest for this track: CHARACTERISTICS=\\\"public.accessibility.describes-spoken-dialog,public.accessibility.describes-music-and-sound\\\" and AUTOSELECT=\\\"YES\\\". Keep the default value, Disabled, if the captions track is not intended to provide such accessibility. MediaConvert will not add the above attributes.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"DISABLED\",\n    \"ENABLED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-webvtt-accessibility-subs-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: WebvttAccessibilitySubs
---
