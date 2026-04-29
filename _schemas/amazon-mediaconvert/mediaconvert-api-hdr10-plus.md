---
description: Setting for HDR10+ metadata insertion
layout: schema
name: Hdr10Plus
properties_list:
- description: ''
  name: MasteringMonitorNits
  type: object
- description: ''
  name: TargetMonitorNits
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hdr10-plus-schema.json
slug: mediaconvert-api-hdr10-plus
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hdr10-plus-schema.json\",\n  \"title\": \"Hdr10Plus\",\n  \"description\": \"Setting for HDR10+ metadata insertion\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MasteringMonitorNits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max4000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"masteringMonitorNits\"\n          },\n          \"description\": \"Specify the HDR10+ mastering display normalized peak luminance, in nits. This is the normalized actual peak luminance of the mastering display, as defined by ST 2094-40.\"\n        }\n      ]\n    },\n    \"TargetMonitorNits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max4000\"\n        },\n        {\n       \
  \   \"xml\": {\n            \"name\": \"targetMonitorNits\"\n          },\n          \"description\": \"Specify the HDR10+ target display nominal peak luminance, in nits. This is the nominal maximum luminance of the target display as defined by ST 2094-40.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hdr10-plus-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Hdr10Plus
---
