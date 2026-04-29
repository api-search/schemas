---
description: 'Specify how MediaConvert writes SegmentTimeline in your output DASH manifest. To write a SegmentTimeline in each video Representation: Keep the default value, Basic. To write a common SegmentTimeline in the video AdaptationSet: Choose Compact. Note that MediaConvert will still write a SegmentTimeline in any Representation that does not share a common timeline. To write a video AdaptationSet for each different output framerate, and a common SegmentTimeline in each AdaptationSet: Choose Distinct.'
layout: schema
name: DashManifestStyle
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dash-manifest-style-schema.json
slug: mediaconvert-api-dash-manifest-style
source_filename: mediaconvert-api-dash-manifest-style-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dash-manifest-style-schema.json\",\n  \"title\": \"DashManifestStyle\",\n  \"description\": \"Specify how MediaConvert writes SegmentTimeline in your output DASH manifest. To write a SegmentTimeline in each video Representation: Keep the default value, Basic. To write a common SegmentTimeline in the video AdaptationSet: Choose Compact. Note that MediaConvert will still write a SegmentTimeline in any Representation that does not share a common timeline. To write a video AdaptationSet for each different output framerate, and a common SegmentTimeline in each AdaptationSet: Choose Distinct.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"BASIC\",\n    \"COMPACT\",\n    \"DISTINCT\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dash-manifest-style-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DashManifestStyle
---
