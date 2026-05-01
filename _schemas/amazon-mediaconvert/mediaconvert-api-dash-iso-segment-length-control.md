---
description: Specify how you want MediaConvert to determine the segment length. Choose Exact (EXACT) to have the encoder use the exact length that you specify with the setting Segment length (SegmentLength). This might result in extra I-frames. Choose Multiple of GOP (GOP_MULTIPLE) to have the encoder round up the segment lengths to match the next GOP boundary.
layout: schema
name: DashIsoSegmentLengthControl
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dash-iso-segment-length-control-schema.json
slug: mediaconvert-api-dash-iso-segment-length-control
source_filename: mediaconvert-api-dash-iso-segment-length-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dash-iso-segment-length-control-schema.json\",\n  \"title\": \"DashIsoSegmentLengthControl\",\n  \"description\": \"Specify how you want MediaConvert to determine the segment length. Choose Exact (EXACT) to have the encoder use the exact length that you specify with the setting Segment length (SegmentLength). This might result in extra I-frames. Choose Multiple of GOP (GOP_MULTIPLE) to have the encoder round up the segment lengths to match the next GOP boundary.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"EXACT\",\n    \"GOP_MULTIPLE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dash-iso-segment-length-control-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DashIsoSegmentLengthControl
---
