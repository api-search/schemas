---
description: Specify whether to flag this audio track as descriptive video service (DVS) in your HLS parent manifest. When you choose Flag (FLAG), MediaConvert includes the parameter CHARACTERISTICS="public.accessibility.describes-video" in the EXT-X-MEDIA entry for this track. When you keep the default choice, Don't flag (DONT_FLAG), MediaConvert leaves this parameter out. The DVS flag can help with accessibility on Apple devices. For more information, see the Apple documentation.
layout: schema
name: CmfcDescriptiveVideoServiceFlag
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-cmfc-descriptive-video-service-flag-schema.json
slug: mediaconvert-api-cmfc-descriptive-video-service-flag
source_filename: mediaconvert-api-cmfc-descriptive-video-service-flag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmfc-descriptive-video-service-flag-schema.json\",\n  \"title\": \"CmfcDescriptiveVideoServiceFlag\",\n  \"description\": \"Specify whether to flag this audio track as descriptive video service (DVS) in your HLS parent manifest. When you choose Flag (FLAG), MediaConvert includes the parameter CHARACTERISTICS=\\\"public.accessibility.describes-video\\\" in the EXT-X-MEDIA entry for this track. When you keep the default choice, Don't flag (DONT_FLAG), MediaConvert leaves this parameter out. The DVS flag can help with accessibility on Apple devices. For more information, see the Apple documentation.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"DONT_FLAG\",\n    \"FLAG\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmfc-descriptive-video-service-flag-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CmfcDescriptiveVideoServiceFlag
---
