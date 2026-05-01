---
description: Use this setting only when your output video stream has B-frames, which causes the initial presentation time stamp (PTS) to be offset from the initial decode time stamp (DTS). Specify how MediaConvert handles PTS when writing time stamps in output DASH manifests. Choose Match initial PTS (MATCH_INITIAL_PTS) when you want MediaConvert to use the initial PTS as the first time stamp in the manifest. Choose Zero-based (ZERO_BASED) to have MediaConvert ignore the initial PTS in the video stream and instead write the initial time stamp as zero in the manifest. For outputs that don't have B-frames, the time stamps in your DASH manifests start at zero regardless of your choice here.
layout: schema
name: CmafPtsOffsetHandlingForBFrames
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-cmaf-pts-offset-handling-for-b-frames-schema.json
slug: mediaconvert-api-cmaf-pts-offset-handling-for-b-frames
source_filename: mediaconvert-api-cmaf-pts-offset-handling-for-b-frames-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-pts-offset-handling-for-b-frames-schema.json\",\n  \"title\": \"CmafPtsOffsetHandlingForBFrames\",\n  \"description\": \"Use this setting only when your output video stream has B-frames, which causes the initial presentation time stamp (PTS) to be offset from the initial decode time stamp (DTS). Specify how MediaConvert handles PTS when writing time stamps in output DASH manifests. Choose Match initial PTS (MATCH_INITIAL_PTS) when you want MediaConvert to use the initial PTS as the first time stamp in the manifest. Choose Zero-based (ZERO_BASED) to have MediaConvert ignore the initial PTS in the video stream and instead write the initial time stamp as zero in the manifest. For outputs that don't have B-frames, the time stamps in your DASH manifests start at zero regardless of\
  \ your choice here.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ZERO_BASED\",\n    \"MATCH_INITIAL_PTS\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-pts-offset-handling-for-b-frames-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CmafPtsOffsetHandlingForBFrames
---
