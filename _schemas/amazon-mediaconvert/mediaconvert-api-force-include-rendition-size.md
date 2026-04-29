---
description: 'Use Force include renditions to specify one or more resolutions to include your ABR stack. * (Recommended) To optimize automated ABR, specify as few resolutions as possible. * (Required) The number of resolutions that you specify must be equal to, or less than, the Max renditions setting. * If you specify a Min top rendition size rule, specify at least one resolution that is equal to, or greater than, Min top rendition size. * If you specify a Min bottom rendition size rule, only specify resolutions that are equal to, or greater than, Min bottom rendition size. * If you specify a Force include renditions rule, do not specify a separate rule for Allowed renditions. * Note: The ABR stack may include other resolutions that you do not specify here, depending on the Max renditions setting.'
layout: schema
name: ForceIncludeRenditionSize
properties_list:
- description: ''
  name: Height
  type: object
- description: ''
  name: Width
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-force-include-rendition-size-schema.json
slug: mediaconvert-api-force-include-rendition-size
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-force-include-rendition-size-schema.json\",\n  \"title\": \"ForceIncludeRenditionSize\",\n  \"description\": \"Use Force include renditions to specify one or more resolutions to include your ABR stack. * (Recommended) To optimize automated ABR, specify as few resolutions as possible. * (Required) The number of resolutions that you specify must be equal to, or less than, the Max renditions setting. * If you specify a Min top rendition size rule, specify at least one resolution that is equal to, or greater than, Min top rendition size. * If you specify a Min bottom rendition size rule, only specify resolutions that are equal to, or greater than, Min bottom rendition size. * If you specify a Force include renditions rule, do not specify a separate rule for Allowed renditions. * Note:\
  \ The ABR stack may include other resolutions that you do not specify here, depending on the Max renditions setting.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Height\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8192\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"height\"\n          },\n          \"description\": \"Use Height to define the video resolution height, in pixels, for this rule.\"\n        }\n      ]\n    },\n    \"Width\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8192\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"width\"\n          },\n          \"description\": \"Use Width to define the video resolution width, in pixels, for this rule.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-force-include-rendition-size-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ForceIncludeRenditionSize
---
