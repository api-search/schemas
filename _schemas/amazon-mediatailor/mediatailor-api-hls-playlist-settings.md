---
description: HLS playlist configuration parameters.
layout: schema
name: HlsPlaylistSettings
properties_list:
- description: ''
  name: ManifestWindowSeconds
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-hls-playlist-settings-schema.json
slug: mediatailor-api-hls-playlist-settings
source_filename: mediatailor-api-hls-playlist-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-hls-playlist-settings-schema.json\",\n  \"title\": \"HlsPlaylistSettings\",\n  \"description\": \"HLS playlist configuration parameters.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ManifestWindowSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"description\": \"The total duration (in seconds) of each manifest. Minimum value: <code>30</code> seconds. Maximum value: <code>3600</code> seconds.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-hls-playlist-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: HlsPlaylistSettings
---
