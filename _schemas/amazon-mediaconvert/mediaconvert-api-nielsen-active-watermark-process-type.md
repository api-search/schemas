---
description: Choose the type of Nielsen watermarks that you want in your outputs. When you choose NAES 2 and NW (NAES2_AND_NW), you must provide a value for the setting SID (sourceId). When you choose CBET (CBET), you must provide a value for the setting CSID (cbetSourceId). When you choose NAES 2, NW, and CBET (NAES2_AND_NW_AND_CBET), you must provide values for both of these settings.
layout: schema
name: NielsenActiveWatermarkProcessType
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-nielsen-active-watermark-process-type-schema.json
slug: mediaconvert-api-nielsen-active-watermark-process-type
source_filename: mediaconvert-api-nielsen-active-watermark-process-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-nielsen-active-watermark-process-type-schema.json\",\n  \"title\": \"NielsenActiveWatermarkProcessType\",\n  \"description\": \"Choose the type of Nielsen watermarks that you want in your outputs. When you choose NAES 2 and NW (NAES2_AND_NW), you must provide a value for the setting SID (sourceId). When you choose CBET (CBET), you must provide a value for the setting CSID (cbetSourceId). When you choose NAES 2, NW, and CBET (NAES2_AND_NW_AND_CBET), you must provide values for both of these settings.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"NAES2_AND_NW\",\n    \"CBET\",\n    \"NAES2_AND_NW_AND_CBET\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-nielsen-active-watermark-process-type-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: NielsenActiveWatermarkProcessType
---
