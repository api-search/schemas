---
description: This setting can improve the compatibility of your output with video players on obsolete devices. It applies only to DASH H.264 outputs with DRM encryption. Choose Unencrypted SEI (UNENCRYPTED_SEI) only to correct problems with playback on older devices. Otherwise, keep the default setting CENC v1 (CENC_V1). If you choose Unencrypted SEI, for that output, the service will exclude the access unit delimiter and will leave the SEI NAL units unencrypted.
layout: schema
name: DashIsoPlaybackDeviceCompatibility
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dash-iso-playback-device-compatibility-schema.json
slug: mediaconvert-api-dash-iso-playback-device-compatibility
source_filename: mediaconvert-api-dash-iso-playback-device-compatibility-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dash-iso-playback-device-compatibility-schema.json\",\n  \"title\": \"DashIsoPlaybackDeviceCompatibility\",\n  \"description\": \"This setting can improve the compatibility of your output with video players on obsolete devices. It applies only to DASH H.264 outputs with DRM encryption. Choose Unencrypted SEI (UNENCRYPTED_SEI) only to correct problems with playback on older devices. Otherwise, keep the default setting CENC v1 (CENC_V1). If you choose Unencrypted SEI, for that output, the service will exclude the access unit delimiter and will leave the SEI NAL units unencrypted.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CENC_V1\",\n    \"UNENCRYPTED_SEI\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dash-iso-playback-device-compatibility-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DashIsoPlaybackDeviceCompatibility
---
