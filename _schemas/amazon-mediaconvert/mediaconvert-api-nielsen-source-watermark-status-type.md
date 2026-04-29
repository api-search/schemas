---
description: Required. Specify whether your source content already contains Nielsen non-linear watermarks. When you set this value to Watermarked (WATERMARKED), the service fails the job. Nielsen requires that you add non-linear watermarking to only clean content that doesn't already have non-linear Nielsen watermarks.
layout: schema
name: NielsenSourceWatermarkStatusType
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-nielsen-source-watermark-status-type-schema.json
slug: mediaconvert-api-nielsen-source-watermark-status-type
source_filename: mediaconvert-api-nielsen-source-watermark-status-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-nielsen-source-watermark-status-type-schema.json\",\n  \"title\": \"NielsenSourceWatermarkStatusType\",\n  \"description\": \"Required. Specify whether your source content already contains Nielsen non-linear watermarks. When you set this value to Watermarked (WATERMARKED), the service fails the job. Nielsen requires that you add non-linear watermarking to only clean content that doesn't already have non-linear Nielsen watermarks.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CLEAN\",\n    \"WATERMARKED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-nielsen-source-watermark-status-type-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: NielsenSourceWatermarkStatusType
---
