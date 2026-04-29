---
description: Use Source (SourceType) to identify the format of your input captions. The service cannot auto-detect caption format.
layout: schema
name: CaptionSourceType
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-caption-source-type-schema.json
slug: mediaconvert-api-caption-source-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-caption-source-type-schema.json\",\n  \"title\": \"CaptionSourceType\",\n  \"description\": \"Use Source (SourceType) to identify the format of your input captions. The service cannot auto-detect caption format.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ANCILLARY\",\n    \"DVB_SUB\",\n    \"EMBEDDED\",\n    \"SCTE20\",\n    \"SCC\",\n    \"TTML\",\n    \"STL\",\n    \"SRT\",\n    \"SMI\",\n    \"SMPTE_TT\",\n    \"TELETEXT\",\n    \"NULL_SOURCE\",\n    \"IMSC\",\n    \"WEBVTT\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-caption-source-type-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CaptionSourceType
---
