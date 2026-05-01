---
description: Specify YUV limits and RGB tolerances when you set Sample range conversion to Limited range clip.
layout: schema
name: ClipLimits
properties_list:
- description: ''
  name: MaximumRGBTolerance
  type: object
- description: ''
  name: MaximumYUV
  type: object
- description: ''
  name: MinimumRGBTolerance
  type: object
- description: ''
  name: MinimumYUV
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-clip-limits-schema.json
slug: mediaconvert-api-clip-limits
source_filename: mediaconvert-api-clip-limits-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-clip-limits-schema.json\",\n  \"title\": \"ClipLimits\",\n  \"description\": \"Specify YUV limits and RGB tolerances when you set Sample range conversion to Limited range clip.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaximumRGBTolerance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin90Max105\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maximumRGBTolerance\"\n          },\n          \"description\": \"Specify the Maximum RGB color sample range tolerance for your output. MediaConvert corrects any YUV values that, when converted to RGB, would be outside the upper tolerance that you specify. Enter an integer from 90 to 105 as an offset percentage to the maximum possible value. Leave blank to use the\
  \ default value 100. When you specify a value for Maximum RGB tolerance, you must set Sample range conversion to Limited range clip.\"\n        }\n      ]\n    },\n    \"MaximumYUV\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin920Max1023\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maximumYUV\"\n          },\n          \"description\": \"Specify the Maximum YUV color sample limit. MediaConvert conforms any pixels in your input above the value that you specify to typical limited range bounds. Enter an integer from 920 to 1023. Leave blank to use the default value 940. The value that you enter applies to 10-bit ranges. For 8-bit ranges, MediaConvert automatically scales this value down. When you specify a value for Maximum YUV, you must set Sample range conversion to Limited range clip.\"\n        }\n      ]\n    },\n    \"MinimumRGBTolerance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative5Max10\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"minimumRGBTolerance\"\n          },\n          \"description\": \"Specify the Minimum RGB color sample range tolerance for your output. MediaConvert corrects any YUV values that, when converted to RGB, would be outside the lower tolerance that you specify. Enter an integer from -5 to 10 as an offset percentage to the minimum possible value. Leave blank to use the default value 0. When you specify a value for Minimum RGB tolerance, you must set Sample range conversion to Limited range clip.\"\n        }\n      ]\n    },\n    \"MinimumYUV\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max128\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"minimumYUV\"\n          },\n          \"description\": \"Specify the Minimum YUV color sample limit. MediaConvert conforms any pixels in your input below the value that you specify to typical limited range bounds.\
  \ Enter an integer from 0 to 128. Leave blank to use the default value 64. The value that you enter applies to 10-bit ranges. For 8-bit ranges, MediaConvert automatically scales this value down. When you specify a value for Minumum YUV, you must set Sample range conversion to Limited range clip.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-clip-limits-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ClipLimits
---
