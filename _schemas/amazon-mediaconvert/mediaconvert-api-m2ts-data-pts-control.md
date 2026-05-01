---
description: If you select ALIGN_TO_VIDEO, MediaConvert writes captions and data packets with Presentation Timestamp (PTS) values greater than or equal to the first video packet PTS (MediaConvert drops captions and data packets with lesser PTS values). Keep the default value (AUTO) to allow all PTS values.
layout: schema
name: M2tsDataPtsControl
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-m2ts-data-pts-control-schema.json
slug: mediaconvert-api-m2ts-data-pts-control
source_filename: mediaconvert-api-m2ts-data-pts-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-data-pts-control-schema.json\",\n  \"title\": \"M2tsDataPtsControl\",\n  \"description\": \"If you select ALIGN_TO_VIDEO, MediaConvert writes captions and data packets with Presentation Timestamp (PTS) values greater than or equal to the first video packet PTS (MediaConvert drops captions and data packets with lesser PTS values). Keep the default value (AUTO) to allow all PTS values.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"AUTO\",\n    \"ALIGN_TO_VIDEO\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-m2ts-data-pts-control-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: M2tsDataPtsControl
---
