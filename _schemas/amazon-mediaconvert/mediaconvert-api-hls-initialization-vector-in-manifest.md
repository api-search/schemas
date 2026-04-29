---
description: The Initialization Vector is a 128-bit number used in conjunction with the key for encrypting blocks. If set to INCLUDE, Initialization Vector is listed in the manifest. Otherwise Initialization Vector is not in the manifest.
layout: schema
name: HlsInitializationVectorInManifest
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-initialization-vector-in-manifest-schema.json
slug: mediaconvert-api-hls-initialization-vector-in-manifest
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-initialization-vector-in-manifest-schema.json\",\n  \"title\": \"HlsInitializationVectorInManifest\",\n  \"description\": \"The Initialization Vector is a 128-bit number used in conjunction with the key for encrypting blocks. If set to INCLUDE, Initialization Vector is listed in the manifest. Otherwise Initialization Vector is not in the manifest.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"INCLUDE\",\n    \"EXCLUDE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-initialization-vector-in-manifest-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsInitializationVectorInManifest
---
