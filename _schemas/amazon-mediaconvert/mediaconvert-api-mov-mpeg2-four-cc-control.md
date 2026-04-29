---
description: When set to XDCAM, writes MPEG2 video streams into the QuickTime file using XDCAM fourcc codes. This increases compatibility with Apple editors and players, but may decrease compatibility with other players. Only applicable when the video codec is MPEG2.
layout: schema
name: MovMpeg2FourCCControl
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-mov-mpeg2-four-cc-control-schema.json
slug: mediaconvert-api-mov-mpeg2-four-cc-control
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mov-mpeg2-four-cc-control-schema.json\",\n  \"title\": \"MovMpeg2FourCCControl\",\n  \"description\": \"When set to XDCAM, writes MPEG2 video streams into the QuickTime file using XDCAM fourcc codes. This increases compatibility with Apple editors and players, but may decrease compatibility with other players. Only applicable when the video codec is MPEG2.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"XDCAM\",\n    \"MPEG\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mov-mpeg2-four-cc-control-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MovMpeg2FourCCControl
---
