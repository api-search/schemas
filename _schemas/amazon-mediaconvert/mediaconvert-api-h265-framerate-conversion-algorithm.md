---
description: Choose the method that you want MediaConvert to use when increasing or decreasing the frame rate. We recommend using drop duplicate (DUPLICATE_DROP) for numerically simple conversions, such as 60 fps to 30 fps. For numerically complex conversions, you can use interpolate (INTERPOLATE) to avoid stutter. This results in a smooth picture, but might introduce undesirable video artifacts. For complex frame rate conversions, especially if your source video has already been converted from its original cadence, use FrameFormer (FRAMEFORMER) to do motion-compensated interpolation. FrameFormer chooses the best conversion method frame by frame. Note that using FrameFormer increases the transcoding time and incurs a significant add-on cost.
layout: schema
name: H265FramerateConversionAlgorithm
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-h265-framerate-conversion-algorithm-schema.json
slug: mediaconvert-api-h265-framerate-conversion-algorithm
source_filename: mediaconvert-api-h265-framerate-conversion-algorithm-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h265-framerate-conversion-algorithm-schema.json\",\n  \"title\": \"H265FramerateConversionAlgorithm\",\n  \"description\": \"Choose the method that you want MediaConvert to use when increasing or decreasing the frame rate. We recommend using drop duplicate (DUPLICATE_DROP) for numerically simple conversions, such as 60 fps to 30 fps. For numerically complex conversions, you can use interpolate (INTERPOLATE) to avoid stutter. This results in a smooth picture, but might introduce undesirable video artifacts. For complex frame rate conversions, especially if your source video has already been converted from its original cadence, use FrameFormer (FRAMEFORMER) to do motion-compensated interpolation. FrameFormer chooses the best conversion method frame by frame. Note that using FrameFormer\
  \ increases the transcoding time and incurs a significant add-on cost.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"DUPLICATE_DROP\",\n    \"INTERPOLATE\",\n    \"FRAMEFORMER\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-h265-framerate-conversion-algorithm-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: H265FramerateConversionAlgorithm
---
