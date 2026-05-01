---
description: Protocol schema from AWS Elemental MediaConnect API
layout: schema
name: Protocol
properties_list: []
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-protocol-schema.json
slug: mediaconnect-api-protocol
source_filename: mediaconnect-api-protocol-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-protocol-schema.json\",\n  \"title\": \"Protocol\",\n  \"description\": \"Protocol schema from AWS Elemental MediaConnect API\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"zixi-push\",\n    \"rtp-fec\",\n    \"rtp\",\n    \"zixi-pull\",\n    \"rist\",\n    \"st2110-jpegxs\",\n    \"cdi\",\n    \"srt-listener\",\n    \"srt-caller\",\n    \"fujitsu-qos\",\n    \"udp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-protocol-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: Protocol
---
