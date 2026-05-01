---
description: Use the image inserter feature to include a graphic overlay on your video. Enable or disable this feature for each input or output individually. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/graphic-overlay.html. This setting is disabled by default.
layout: schema
name: ImageInserter
properties_list:
- description: ''
  name: InsertableImages
  type: object
- description: ''
  name: SdrReferenceWhiteLevel
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-image-inserter-schema.json
slug: mediaconvert-api-image-inserter
source_filename: mediaconvert-api-image-inserter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-image-inserter-schema.json\",\n  \"title\": \"ImageInserter\",\n  \"description\": \"Use the image inserter feature to include a graphic overlay on your video. Enable or disable this feature for each input or output individually. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/graphic-overlay.html. This setting is disabled by default.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InsertableImages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfInsertableImage\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"insertableImages\"\n          },\n          \"description\": \"Specify the images that you want to overlay on your video. The images must be PNG or TGA files.\"\n        }\n   \
  \   ]\n    },\n    \"SdrReferenceWhiteLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin100Max1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sdrReferenceWhiteLevel\"\n          },\n          \"description\": \"Specify the reference white level, in nits, for all of your image inserter images. Use to correct brightness levels within HDR10 outputs. For 1,000 nit peak brightness displays, we recommend that you set SDR reference white level to 203 (according to ITU-R BT.2408). Leave blank to use the default value of 100, or specify an integer from 100 to 1000.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-image-inserter-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ImageInserter
---
