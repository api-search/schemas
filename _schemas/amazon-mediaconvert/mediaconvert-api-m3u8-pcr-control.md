---
description: When set to PCR_EVERY_PES_PACKET a Program Clock Reference value is inserted for every Packetized Elementary Stream (PES) header. This parameter is effective only when the PCR PID is the same as the video or audio elementary stream.
layout: schema
name: M3u8PcrControl
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-m3u8-pcr-control-schema.json
slug: mediaconvert-api-m3u8-pcr-control
source_filename: mediaconvert-api-m3u8-pcr-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m3u8-pcr-control-schema.json\",\n  \"title\": \"M3u8PcrControl\",\n  \"description\": \"When set to PCR_EVERY_PES_PACKET a Program Clock Reference value is inserted for every Packetized Elementary Stream (PES) header. This parameter is effective only when the PCR PID is the same as the video or audio elementary stream.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PCR_EVERY_PES_PACKET\",\n    \"CONFIGURED_PCR_PERIOD\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m3u8-pcr-control-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: M3u8PcrControl
---
