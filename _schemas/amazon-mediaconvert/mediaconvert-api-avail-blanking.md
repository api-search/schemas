---
description: Use ad avail blanking settings to specify your output content during SCTE-35 triggered ad avails. You can blank your video or overlay it with an image. MediaConvert also removes any audio and embedded captions during the ad avail. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/ad-avail-blanking.html.
layout: schema
name: AvailBlanking
properties_list:
- description: ''
  name: AvailBlankingImage
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-avail-blanking-schema.json
slug: mediaconvert-api-avail-blanking
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-avail-blanking-schema.json\",\n  \"title\": \"AvailBlanking\",\n  \"description\": \"Use ad avail blanking settings to specify your output content during SCTE-35 triggered ad avails. You can blank your video or overlay it with an image. MediaConvert also removes any audio and embedded captions during the ad avail. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/ad-avail-blanking.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AvailBlankingImage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin14PatternS3BmpBMPPngPNGHttpsBmpBMPPngPNG\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"availBlankingImage\"\n          },\n          \"description\": \"Blanking image to be used. Leave\
  \ empty for solid black. Only bmp and png images are supported.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-avail-blanking-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AvailBlanking
---
