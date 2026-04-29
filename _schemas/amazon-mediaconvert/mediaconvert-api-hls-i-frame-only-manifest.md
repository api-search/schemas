---
description: Choose Include (INCLUDE) to have MediaConvert generate a child manifest that lists only the I-frames for this rendition, in addition to your regular manifest for this rendition. You might use this manifest as part of a workflow that creates preview functions for your video. MediaConvert adds both the I-frame only child manifest and the regular child manifest to the parent manifest. When you don't need the I-frame only child manifest, keep the default value Exclude (EXCLUDE).
layout: schema
name: HlsIFrameOnlyManifest
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-i-frame-only-manifest-schema.json
slug: mediaconvert-api-hls-i-frame-only-manifest
source_filename: mediaconvert-api-hls-i-frame-only-manifest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-i-frame-only-manifest-schema.json\",\n  \"title\": \"HlsIFrameOnlyManifest\",\n  \"description\": \"Choose Include (INCLUDE) to have MediaConvert generate a child manifest that lists only the I-frames for this rendition, in addition to your regular manifest for this rendition. You might use this manifest as part of a workflow that creates preview functions for your video. MediaConvert adds both the I-frame only child manifest and the regular child manifest to the parent manifest. When you don't need the I-frame only child manifest, keep the default value Exclude (EXCLUDE).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"INCLUDE\",\n    \"EXCLUDE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-i-frame-only-manifest-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsIFrameOnlyManifest
---
