---
description: 'Specify how the value for bandwidth is determined for each video Representation in your output MPD manifest. We recommend that you choose a MPD manifest bandwidth type that is compatible with your downstream player configuration. Max: Use the same value that you specify for Max bitrate in the video output, in bits per second. Average: Use the calculated average bitrate of the encoded video output, in bits per second.'
layout: schema
name: DashIsoMpdManifestBandwidthType
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dash-iso-mpd-manifest-bandwidth-type-schema.json
slug: mediaconvert-api-dash-iso-mpd-manifest-bandwidth-type
source_filename: mediaconvert-api-dash-iso-mpd-manifest-bandwidth-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dash-iso-mpd-manifest-bandwidth-type-schema.json\",\n  \"title\": \"DashIsoMpdManifestBandwidthType\",\n  \"description\": \"Specify how the value for bandwidth is determined for each video Representation in your output MPD manifest. We recommend that you choose a MPD manifest bandwidth type that is compatible with your downstream player configuration. Max: Use the same value that you specify for Max bitrate in the video output, in bits per second. Average: Use the calculated average bitrate of the encoded video output, in bits per second.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"AVERAGE\",\n    \"MAX\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dash-iso-mpd-manifest-bandwidth-type-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DashIsoMpdManifestBandwidthType
---
