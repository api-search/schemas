---
description: 'Specify the color space you want for this output. The service supports conversion between HDR formats, between SDR formats, from SDR to HDR, and from HDR to SDR. SDR to HDR conversion doesn''t upgrade the dynamic range. The converted video has an HDR format, but visually appears the same as an unconverted output. HDR to SDR conversion uses tone mapping to approximate the outcome of manually regrading from HDR to SDR. When you specify an output color space, MediaConvert uses the following color space metadata, which includes color primaries, transfer characteristics, and matrix coefficients: * HDR 10: BT.2020, PQ, BT.2020 non-constant * HLG 2020: BT.2020, HLG, BT.2020 non-constant * P3DCI (Theater): DCIP3, SMPTE 428M, BT.709 * P3D65 (SDR): Display P3, sRGB, BT.709 * P3D65 (HDR): Display P3, PQ, BT.709'
layout: schema
name: ColorSpaceConversion
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-color-space-conversion-schema.json
slug: mediaconvert-api-color-space-conversion
source_filename: mediaconvert-api-color-space-conversion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-color-space-conversion-schema.json\",\n  \"title\": \"ColorSpaceConversion\",\n  \"description\": \"Specify the color space you want for this output. The service supports conversion between HDR formats, between SDR formats, from SDR to HDR, and from HDR to SDR. SDR to HDR conversion doesn't upgrade the dynamic range. The converted video has an HDR format, but visually appears the same as an unconverted output. HDR to SDR conversion uses tone mapping to approximate the outcome of manually regrading from HDR to SDR. When you specify an output color space, MediaConvert uses the following color space metadata, which includes color primaries, transfer characteristics, and matrix coefficients:\\n  * HDR 10: BT.2020, PQ, BT.2020 non-constant\\n  * HLG 2020: BT.2020, HLG, BT.2020 non-constant\\\
  n  * P3DCI (Theater): DCIP3, SMPTE 428M, BT.709\\n  * P3D65 (SDR): Display P3, sRGB, BT.709\\n  * P3D65 (HDR): Display P3, PQ, BT.709\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"NONE\",\n    \"FORCE_601\",\n    \"FORCE_709\",\n    \"FORCE_HDR10\",\n    \"FORCE_HLG_2020\",\n    \"FORCE_P3DCI\",\n    \"FORCE_P3D65_SDR\",\n    \"FORCE_P3D65_HDR\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-color-space-conversion-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ColorSpaceConversion
---
