---
description: Encrypts the segments with the given encryption scheme. Leave blank to disable. Selecting 'Disabled' in the web interface also disables encryption.
layout: schema
name: HlsEncryptionType
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-hls-encryption-type-schema.json
slug: mediaconvert-api-hls-encryption-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-encryption-type-schema.json\",\n  \"title\": \"HlsEncryptionType\",\n  \"description\": \"Encrypts the segments with the given encryption scheme. Leave blank to disable. Selecting 'Disabled' in the web interface also disables encryption.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"AES128\",\n    \"SAMPLE_AES\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-hls-encryption-type-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HlsEncryptionType
---
