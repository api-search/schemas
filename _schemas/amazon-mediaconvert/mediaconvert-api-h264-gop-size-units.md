---
description: Specify how the transcoder determines GOP size for this output. We recommend that you have the transcoder automatically choose this value for you based on characteristics of your input video. To enable this automatic behavior, choose Auto (AUTO) and and leave GOP size (GopSize) blank. By default, if you don't specify GOP mode control (GopSizeUnits), MediaConvert will use automatic behavior. If your output group specifies HLS, DASH, or CMAF, set GOP mode control to Auto and leave GOP size blank in each output in your output group. To explicitly specify the GOP length, choose Specified, frames (FRAMES) or Specified, seconds (SECONDS) and then provide the GOP length in the related setting GOP size (GopSize).
layout: schema
name: H264GopSizeUnits
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-h264-gop-size-units-schema.json
slug: mediaconvert-api-h264-gop-size-units
source_filename: mediaconvert-api-h264-gop-size-units-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h264-gop-size-units-schema.json\",\n  \"title\": \"H264GopSizeUnits\",\n  \"description\": \"Specify how the transcoder determines GOP size for this output. We recommend that you have the transcoder automatically choose this value for you based on characteristics of your input video. To enable this automatic behavior, choose Auto (AUTO) and and leave GOP size (GopSize) blank. By default, if you don't specify GOP mode control (GopSizeUnits), MediaConvert will use automatic behavior. If your output group specifies HLS, DASH, or CMAF, set GOP mode control to Auto and leave GOP size blank in each output in your output group. To explicitly specify the GOP length, choose Specified, frames (FRAMES) or Specified, seconds (SECONDS) and then provide the GOP length in the related setting GOP\
  \ size (GopSize).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"FRAMES\",\n    \"SECONDS\",\n    \"AUTO\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h264-gop-size-units-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: H264GopSizeUnits
---
