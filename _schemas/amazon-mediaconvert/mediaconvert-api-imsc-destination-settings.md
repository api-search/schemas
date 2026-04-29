---
description: Settings related to IMSC captions. IMSC is a sidecar format that holds captions in a file that is separate from the video container. Set up sidecar captions in the same output group, but different output from your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/ttml-and-webvtt-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to IMSC.
layout: schema
name: ImscDestinationSettings
properties_list:
- description: ''
  name: Accessibility
  type: object
- description: ''
  name: StylePassthrough
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-imsc-destination-settings-schema.json
slug: mediaconvert-api-imsc-destination-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-imsc-destination-settings-schema.json\",\n  \"title\": \"ImscDestinationSettings\",\n  \"description\": \"Settings related to IMSC captions. IMSC is a sidecar format that holds captions in a file that is separate from the video container. Set up sidecar captions in the same output group, but different output from your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/ttml-and-webvtt-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to IMSC.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Accessibility\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImscAccessibilitySubs\"\n        },\n        {\n          \"\
  xml\": {\n            \"name\": \"accessibility\"\n          },\n          \"description\": \"Set Accessibility subtitles to Enabled if the ISMC or WebVTT captions track is intended to provide accessibility for people who are deaf or hard of hearing. When you enable this feature, MediaConvert adds the following attributes under EXT-X-MEDIA in the HLS or CMAF manifest for this track: CHARACTERISTICS=\\\"public.accessibility.describes-spoken-dialog,public.accessibility.describes-music-and-sound\\\" and AUTOSELECT=\\\"YES\\\". Keep the default value, Disabled, if the captions track is not intended to provide such accessibility. MediaConvert will not add the above attributes.\"\n        }\n      ]\n    },\n    \"StylePassthrough\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImscStylePassthrough\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"stylePassthrough\"\n          },\n          \"description\": \"Keep this setting enabled to\
  \ have MediaConvert use the font style and position information from the captions source in the output. This option is available only when your input captions are IMSC, SMPTE-TT, or TTML. Disable this setting for simplified output captions.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-imsc-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ImscDestinationSettings
---
