---
description: 'To include key-length-value metadata in this output: Set KLV metadata insertion to Passthrough. MediaConvert reads KLV metadata present in your input and passes it through to the output transport stream. To exclude this KLV metadata: Set KLV metadata insertion to None or leave blank.'
layout: schema
name: M2tsKlvMetadata
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-m2ts-klv-metadata-schema.json
slug: mediaconvert-api-m2ts-klv-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-klv-metadata-schema.json\",\n  \"title\": \"M2tsKlvMetadata\",\n  \"description\": \"To include key-length-value metadata in this output: Set KLV metadata insertion to Passthrough. MediaConvert reads KLV metadata present in your input and passes it through to the output transport stream. To exclude this KLV metadata: Set KLV metadata insertion to None or leave blank.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PASSTHROUGH\",\n    \"NONE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-klv-metadata-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: M2tsKlvMetadata
---
