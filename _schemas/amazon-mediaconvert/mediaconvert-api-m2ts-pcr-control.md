---
description: When set to PCR_EVERY_PES_PACKET, a Program Clock Reference value is inserted for every Packetized Elementary Stream (PES) header. This is effective only when the PCR PID is the same as the video or audio elementary stream.
layout: schema
name: M2tsPcrControl
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-m2ts-pcr-control-schema.json
slug: mediaconvert-api-m2ts-pcr-control
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-pcr-control-schema.json\",\n  \"title\": \"M2tsPcrControl\",\n  \"description\": \"When set to PCR_EVERY_PES_PACKET, a Program Clock Reference value is inserted for every Packetized Elementary Stream (PES) header. This is effective only when the PCR PID is the same as the video or audio elementary stream.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PCR_EVERY_PES_PACKET\",\n    \"CONFIGURED_PCR_PERIOD\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-pcr-control-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: M2tsPcrControl
---
