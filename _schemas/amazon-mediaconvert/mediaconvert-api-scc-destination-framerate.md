---
description: Set Framerate (SccDestinationFramerate) to make sure that the captions and the video are synchronized in the output. Specify a frame rate that matches the frame rate of the associated video. If the video frame rate is 29.97, choose 29.97 dropframe (FRAMERATE_29_97_DROPFRAME) only if the video has video_insertion=true and drop_frame_timecode=true; otherwise, choose 29.97 non-dropframe (FRAMERATE_29_97_NON_DROPFRAME).
layout: schema
name: SccDestinationFramerate
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-scc-destination-framerate-schema.json
slug: mediaconvert-api-scc-destination-framerate
source_filename: mediaconvert-api-scc-destination-framerate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-scc-destination-framerate-schema.json\",\n  \"title\": \"SccDestinationFramerate\",\n  \"description\": \"Set Framerate (SccDestinationFramerate) to make sure that the captions and the video are synchronized in the output. Specify a frame rate that matches the frame rate of the associated video. If the video frame rate is 29.97, choose 29.97 dropframe (FRAMERATE_29_97_DROPFRAME) only if the video has video_insertion=true and drop_frame_timecode=true; otherwise, choose 29.97 non-dropframe (FRAMERATE_29_97_NON_DROPFRAME).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"FRAMERATE_23_97\",\n    \"FRAMERATE_24\",\n    \"FRAMERATE_25\",\n    \"FRAMERATE_29_97_DROPFRAME\",\n    \"FRAMERATE_29_97_NON_DROPFRAME\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-scc-destination-framerate-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: SccDestinationFramerate
---
