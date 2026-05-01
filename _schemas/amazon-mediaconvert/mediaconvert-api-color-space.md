---
description: 'If your input video has accurate color space metadata, or if you don''t know about color space: Keep the default value, Follow. MediaConvert will automatically detect your input color space. If your input video has metadata indicating the wrong color space, or has missing metadata: Specify the accurate color space here. If your input video is HDR 10 and the SMPTE ST 2086 Mastering Display Color Volume static metadata isn''t present in your video stream, or if that metadata is present but not accurate: Choose Force HDR 10. Specify correct values in the input HDR 10 metadata settings. For more information about HDR jobs, see https://docs.aws.amazon.com/console/mediaconvert/hdr. When you specify an input color space, MediaConvert uses the following color space metadata, which includes color primaries, transfer characteristics, and matrix coefficients: * HDR 10: BT.2020, PQ, BT.2020 non-constant * HLG 2020: BT.2020, HLG, BT.2020 non-constant * P3DCI (Theater): DCIP3, SMPTE 428M,
  BT.709 * P3D65 (SDR): Display P3, sRGB, BT.709 * P3D65 (HDR): Display P3, PQ, BT.709'
layout: schema
name: ColorSpace
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-color-space-schema.json
slug: mediaconvert-api-color-space
source_filename: mediaconvert-api-color-space-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-color-space-schema.json\",\n  \"title\": \"ColorSpace\",\n  \"description\": \"If your input video has accurate color space metadata, or if you don't know about color space: Keep the default value, Follow. MediaConvert will automatically detect your input color space. If your input video has metadata indicating the wrong color space, or has missing metadata: Specify the accurate color space here. If your input video is HDR 10 and the SMPTE ST 2086 Mastering Display Color Volume static metadata isn't present in your video stream, or if that metadata is present but not accurate: Choose Force HDR 10. Specify correct values in the input HDR 10 metadata settings. For more information about HDR jobs, see https://docs.aws.amazon.com/console/mediaconvert/hdr. When you specify an input color\
  \ space, MediaConvert uses the following color space metadata, which includes color primaries, transfer characteristics, and matrix coefficients:\\n * HDR 10: BT.2020, PQ, BT.2020 non-constant\\n * HLG 2020: BT.2020, HLG, BT.2020 non-constant\\n * P3DCI (Theater): DCIP3, SMPTE 428M, BT.709\\n * P3D65 (SDR): Display P3, sRGB, BT.709\\n * P3D65 (HDR): Display P3, PQ, BT.709\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"FOLLOW\",\n    \"REC_601\",\n    \"REC_709\",\n    \"HDR10\",\n    \"HLG_2020\",\n    \"P3DCI\",\n    \"P3D65_SDR\",\n    \"P3D65_HDR\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-color-space-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ColorSpace
---
