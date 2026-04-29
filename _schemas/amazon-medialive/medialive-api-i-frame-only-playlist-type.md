---
description: When set to "standard", an I-Frame only playlist will be written out for each video output in the output group. This I-Frame only playlist will contain byte range offsets pointing to the I-frame(s) in each segment.
layout: schema
name: IFrameOnlyPlaylistType
properties_list: []
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-i-frame-only-playlist-type-schema.json
slug: medialive-api-i-frame-only-playlist-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-i-frame-only-playlist-type-schema.json\",\n  \"title\": \"IFrameOnlyPlaylistType\",\n  \"description\": \"When set to \\\"standard\\\", an I-Frame only playlist will be written out for each video output in the output group. This I-Frame only playlist will contain byte range offsets pointing to the I-frame(s) in each segment.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"DISABLED\",\n    \"STANDARD\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-i-frame-only-playlist-type-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: IFrameOnlyPlaylistType
---
