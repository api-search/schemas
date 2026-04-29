---
description: 'Optional. Choose Include (INCLUDE) to have MediaConvert mark up your DASH manifest with <Accessibility> elements for embedded 608 captions. This markup isn''t generally required, but some video players require it to discover and play embedded 608 captions. Keep the default value, Exclude (EXCLUDE), to leave these elements out. When you enable this setting, this is the markup that MediaConvert includes in your manifest: <Accessibility schemeIdUri="urn:scte:dash:cc:cea-608:2015" value="CC1=eng"/>'
layout: schema
name: MpdAccessibilityCaptionHints
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-mpd-accessibility-caption-hints-schema.json
slug: mediaconvert-api-mpd-accessibility-caption-hints
source_filename: mediaconvert-api-mpd-accessibility-caption-hints-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mpd-accessibility-caption-hints-schema.json\",\n  \"title\": \"MpdAccessibilityCaptionHints\",\n  \"description\": \"Optional. Choose Include (INCLUDE) to have MediaConvert mark up your DASH manifest with <Accessibility> elements for embedded 608 captions. This markup isn't generally required, but some video players require it to discover and play embedded 608 captions. Keep the default value, Exclude (EXCLUDE), to leave these elements out. When you enable this setting, this is the markup that MediaConvert includes in your manifest: <Accessibility schemeIdUri=\\\"urn:scte:dash:cc:cea-608:2015\\\" value=\\\"CC1=eng\\\"/>\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"INCLUDE\",\n    \"EXCLUDE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mpd-accessibility-caption-hints-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MpdAccessibilityCaptionHints
---
