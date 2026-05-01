---
description: Set Caption segment length control (CaptionSegmentLengthControl) to Match video (MATCH_VIDEO) to create caption segments that align with the video segments from the first video output in this output group. For example, if the video segments are 2 seconds long, your WebVTT segments will also be 2 seconds long. Keep the default setting, Large segments (LARGE_SEGMENTS) to create caption segments that are 300 seconds long.
layout: schema
name: HlsCaptionSegmentLengthControl
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-caption-segment-length-control-schema.json
slug: mediaconvert-api-hls-caption-segment-length-control
source_filename: mediaconvert-api-hls-caption-segment-length-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-caption-segment-length-control-schema.json\",\n  \"title\": \"HlsCaptionSegmentLengthControl\",\n  \"description\": \"Set Caption segment length control (CaptionSegmentLengthControl) to Match video (MATCH_VIDEO) to create caption segments that align with the video segments from the first video output in this output group. For example, if the video segments are 2 seconds long, your WebVTT segments will also be 2 seconds long. Keep the default setting, Large segments (LARGE_SEGMENTS) to create caption segments that are 300 seconds long.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"LARGE_SEGMENTS\",\n    \"MATCH_VIDEO\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-caption-segment-length-control-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: HlsCaptionSegmentLengthControl
---
