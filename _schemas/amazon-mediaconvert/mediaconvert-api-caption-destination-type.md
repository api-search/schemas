---
description: Specify the format for this set of captions on this output. The default format is embedded without SCTE-20. Note that your choice of video output container constrains your choice of output captions format. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/captions-support-tables.html. If you are using SCTE-20 and you want to create an output that complies with the SCTE-43 spec, choose SCTE-20 plus embedded (SCTE20_PLUS_EMBEDDED). To create a non-compliant output where the embedded captions come first, choose Embedded plus SCTE-20 (EMBEDDED_PLUS_SCTE20).
layout: schema
name: CaptionDestinationType
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-caption-destination-type-schema.json
slug: mediaconvert-api-caption-destination-type
source_filename: mediaconvert-api-caption-destination-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-caption-destination-type-schema.json\",\n  \"title\": \"CaptionDestinationType\",\n  \"description\": \"Specify the format for this set of captions on this output. The default format is embedded without SCTE-20. Note that your choice of video output container constrains your choice of output captions format. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/captions-support-tables.html. If you are using SCTE-20 and you want to create an output that complies with the SCTE-43 spec, choose SCTE-20 plus embedded (SCTE20_PLUS_EMBEDDED). To create a non-compliant output where the embedded captions come first, choose Embedded plus SCTE-20 (EMBEDDED_PLUS_SCTE20).\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"BURN_IN\",\n    \"DVB_SUB\",\n    \"EMBEDDED\",\n \
  \   \"EMBEDDED_PLUS_SCTE20\",\n    \"IMSC\",\n    \"SCTE20_PLUS_EMBEDDED\",\n    \"SCC\",\n    \"SRT\",\n    \"SMI\",\n    \"TELETEXT\",\n    \"TTML\",\n    \"WEBVTT\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-caption-destination-type-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CaptionDestinationType
---
