---
description: Controls what buffer model to use for accurate interleaving. If set to MULTIPLEX, use multiplex buffer model. If set to NONE, this can lead to lower latency, but low-memory devices may not be able to play back the stream without interruptions.
layout: schema
name: M2tsBufferModel
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-m2ts-buffer-model-schema.json
slug: mediaconvert-api-m2ts-buffer-model
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-buffer-model-schema.json\",\n  \"title\": \"M2tsBufferModel\",\n  \"description\": \"Controls what buffer model to use for accurate interleaving. If set to MULTIPLEX, use multiplex buffer model. If set to NONE, this can lead to lower latency, but low-memory devices may not be able to play back the stream without interruptions.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"MULTIPLEX\",\n    \"NONE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-buffer-model-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: M2tsBufferModel
---
