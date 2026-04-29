---
description: Specify the AVC-Intra class of your output. The AVC-Intra class selection determines the output video bit rate depending on the frame rate of the output. Outputs with higher class values have higher bitrates and improved image quality. Note that for Class 4K/2K, MediaConvert supports only 4:2:2 chroma subsampling.
layout: schema
name: AvcIntraClass
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-avc-intra-class-schema.json
slug: mediaconvert-api-avc-intra-class
source_filename: mediaconvert-api-avc-intra-class-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-avc-intra-class-schema.json\",\n  \"title\": \"AvcIntraClass\",\n  \"description\": \"Specify the AVC-Intra class of your output. The AVC-Intra class selection determines the output video bit rate depending on the frame rate of the output. Outputs with higher class values have higher bitrates and improved image quality. Note that for Class 4K/2K, MediaConvert supports only 4:2:2 chroma subsampling.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CLASS_50\",\n    \"CLASS_100\",\n    \"CLASS_200\",\n    \"CLASS_4K_2K\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-avc-intra-class-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AvcIntraClass
---
