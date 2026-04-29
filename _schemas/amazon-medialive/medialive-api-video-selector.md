---
description: Specifies a particular video stream within an input source. An input may have only a single video selector.
layout: schema
name: VideoSelector
properties_list:
- description: ''
  name: ColorSpace
  type: object
- description: ''
  name: ColorSpaceSettings
  type: object
- description: ''
  name: ColorSpaceUsage
  type: object
- description: ''
  name: SelectorSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-video-selector-schema.json
slug: medialive-api-video-selector
source_filename: medialive-api-video-selector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-selector-schema.json\",\n  \"title\": \"VideoSelector\",\n  \"description\": \"Specifies a particular video stream within an input source. An input may have only a single video selector.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ColorSpace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoSelectorColorSpace\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"colorSpace\"\n          },\n          \"description\": \"Specifies the color space of an input. This setting works in tandem with colorSpaceUsage and a video description's colorSpaceSettingsChoice to determine if any conversion will be performed.\"\n        }\n      ]\n    },\n    \"ColorSpaceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/VideoSelectorColorSpaceSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"colorSpaceSettings\"\n          },\n          \"description\": \"Color space settings\"\n        }\n      ]\n    },\n    \"ColorSpaceUsage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoSelectorColorSpaceUsage\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"colorSpaceUsage\"\n          },\n          \"description\": \"Applies only if colorSpace is a value other than follow. This field controls how the value in the colorSpace field will be used. fallback means that when the input does include color space data, that data will be used, but when the input has no color space data, the value in colorSpace will be used. Choose fallback if your input is sometimes missing color space data, but when it does have color space data, that data is correct. force means to always use the value in colorSpace. Choose force\
  \ if your input usually has no color space data or might have unreliable color space data.\"\n        }\n      ]\n    },\n    \"SelectorSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VideoSelectorSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"selectorSettings\"\n          },\n          \"description\": \"The video selector settings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-video-selector-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: VideoSelector
---
