---
description: Settings related to SCC captions. SCC is a sidecar format that holds captions in a file that is separate from the video container. Set up sidecar captions in the same output group, but different output from your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/scc-srt-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to SCC.
layout: schema
name: SccDestinationSettings
properties_list:
- description: ''
  name: Framerate
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-scc-destination-settings-schema.json
slug: mediaconvert-api-scc-destination-settings
source_filename: mediaconvert-api-scc-destination-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-scc-destination-settings-schema.json\",\n  \"title\": \"SccDestinationSettings\",\n  \"description\": \"Settings related to SCC captions. SCC is a sidecar format that holds captions in a file that is separate from the video container. Set up sidecar captions in the same output group, but different output from your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/scc-srt-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to SCC.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Framerate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SccDestinationFramerate\"\n        },\n        {\n          \"xml\": {\n     \
  \       \"name\": \"framerate\"\n          },\n          \"description\": \"Set Framerate (SccDestinationFramerate) to make sure that the captions and the video are synchronized in the output. Specify a frame rate that matches the frame rate of the associated video. If the video frame rate is 29.97, choose 29.97 dropframe (FRAMERATE_29_97_DROPFRAME) only if the video has video_insertion=true and drop_frame_timecode=true; otherwise, choose 29.97 non-dropframe (FRAMERATE_29_97_NON_DROPFRAME).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-scc-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: SccDestinationSettings
---
