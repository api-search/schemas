---
description: Settings related to WebVTT captions. WebVTT is a sidecar format that holds captions in a file that is separate from the video container. Set up sidecar captions in the same output group, but different output from your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/ttml-and-webvtt-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to WebVTT.
layout: schema
name: WebvttDestinationSettings
properties_list:
- description: ''
  name: Accessibility
  type: object
- description: ''
  name: StylePassthrough
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-webvtt-destination-settings-schema.json
slug: mediaconvert-api-webvtt-destination-settings
source_filename: mediaconvert-api-webvtt-destination-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-webvtt-destination-settings-schema.json\",\n  \"title\": \"WebvttDestinationSettings\",\n  \"description\": \"Settings related to WebVTT captions. WebVTT is a sidecar format that holds captions in a file that is separate from the video container. Set up sidecar captions in the same output group, but different output from your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/ttml-and-webvtt-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to WebVTT.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Accessibility\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebvttAccessibilitySubs\"\n        },\n        {\n\
  \          \"xml\": {\n            \"name\": \"accessibility\"\n          },\n          \"description\": \"Set Accessibility subtitles to Enabled if the ISMC or WebVTT captions track is intended to provide accessibility for people who are deaf or hard of hearing. When you enable this feature, MediaConvert adds the following attributes under EXT-X-MEDIA in the HLS or CMAF manifest for this track: CHARACTERISTICS=\\\"public.accessibility.describes-spoken-dialog,public.accessibility.describes-music-and-sound\\\" and AUTOSELECT=\\\"YES\\\". Keep the default value, Disabled, if the captions track is not intended to provide such accessibility. MediaConvert will not add the above attributes.\"\n        }\n      ]\n    },\n    \"StylePassthrough\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WebvttStylePassthrough\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"stylePassthrough\"\n          },\n          \"description\": \"To use the available\
  \ style, color, and position information from your input captions: Set Style passthrough (stylePassthrough) to Enabled (ENABLED). MediaConvert uses default settings when style and position information is missing from your input captions. To recreate the input captions exactly: Set Style passthrough to Strict (STRICT). MediaConvert automatically applies timing adjustments, including adjustments for frame rate conversion, ad avails, and input clipping. Your input captions format must be WebVTT. To ignore the style and position information from your input captions and use simplified output captions: Set Style passthrough to Disabled (DISABLED), or leave blank.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-webvtt-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: WebvttDestinationSettings
---
