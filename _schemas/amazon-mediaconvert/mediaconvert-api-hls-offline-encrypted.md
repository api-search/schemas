---
description: Enable this setting to insert the EXT-X-SESSION-KEY element into the master playlist. This allows for offline Apple HLS FairPlay content protection.
layout: schema
name: HlsOfflineEncrypted
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-offline-encrypted-schema.json
slug: mediaconvert-api-hls-offline-encrypted
source_filename: mediaconvert-api-hls-offline-encrypted-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-offline-encrypted-schema.json\",\n  \"title\": \"HlsOfflineEncrypted\",\n  \"description\": \"Enable this setting to insert the EXT-X-SESSION-KEY element into the master playlist. This allows for offline Apple HLS FairPlay content protection.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ENABLED\",\n    \"DISABLED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-offline-encrypted-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsOfflineEncrypted
---
