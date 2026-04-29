---
description: Use Allowed renditions to specify a list of possible resolutions in your ABR stack. * MediaConvert will create an ABR stack exclusively from the list of resolutions that you specify. * Some resolutions in the Allowed renditions list may not be included, however you can force a resolution to be included by setting Required to ENABLED. * You must specify at least one resolution that is greater than or equal to any resolutions that you specify in Min top rendition size or Min bottom rendition size. * If you specify Allowed renditions, you must not specify a separate rule for Force include renditions.
layout: schema
name: AllowedRenditionSize
properties_list:
- description: ''
  name: Height
  type: object
- description: ''
  name: Required
  type: object
- description: ''
  name: Width
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-allowed-rendition-size-schema.json
slug: mediaconvert-api-allowed-rendition-size
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-allowed-rendition-size-schema.json\",\n  \"title\": \"AllowedRenditionSize\",\n  \"description\": \"Use Allowed renditions to specify a list of possible resolutions in your ABR stack. * MediaConvert will create an ABR stack exclusively from the list of resolutions that you specify. * Some resolutions in the Allowed renditions list may not be included, however you can force a resolution to be included by setting Required to ENABLED. * You must specify at least one resolution that is greater than or equal to any resolutions that you specify in Min top rendition size or Min bottom rendition size. * If you specify Allowed renditions, you must not specify a separate rule for Force include renditions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Height\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8192\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"height\"\n          },\n          \"description\": \"Use Height to define the video resolution height, in pixels, for this rule.\"\n        }\n      ]\n    },\n    \"Required\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequiredFlag\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"required\"\n          },\n          \"description\": \"Set to ENABLED to force a rendition to be included.\"\n        }\n      ]\n    },\n    \"Width\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin32Max8192\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"width\"\n          },\n          \"description\": \"Use Width to define the video resolution width, in pixels, for this rule.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-allowed-rendition-size-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AllowedRenditionSize
---
