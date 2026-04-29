---
description: 'Choose the Dolby dynamic range control (DRC) profile that MediaConvert uses when encoding the metadata in the Dolby stream for the RF operating mode. Default value: Film light (ATMOS_STORAGE_DDP_COMPR_FILM_LIGHT) Related setting: To have MediaConvert use the value you specify here, keep the default value, Custom (SPECIFIED) for the setting Dynamic range control (DynamicRangeControl). Otherwise, MediaConvert ignores Dynamic range compression RF (DynamicRangeCompressionRf). For information about the Dolby DRC operating modes and profiles, see the Dynamic Range Control chapter of the Dolby Metadata Guide at https://developer.dolby.com/globalassets/professional/documents/dolby-metadata-guide.pdf.'
layout: schema
name: Eac3AtmosDynamicRangeCompressionRf
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-eac3-atmos-dynamic-range-compression-rf-schema.json
slug: mediaconvert-api-eac3-atmos-dynamic-range-compression-rf
source_filename: mediaconvert-api-eac3-atmos-dynamic-range-compression-rf-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-atmos-dynamic-range-compression-rf-schema.json\",\n  \"title\": \"Eac3AtmosDynamicRangeCompressionRf\",\n  \"description\": \"Choose the Dolby dynamic range control (DRC) profile that MediaConvert uses when encoding the metadata in the Dolby stream for the RF operating mode. Default value: Film light (ATMOS_STORAGE_DDP_COMPR_FILM_LIGHT) Related setting: To have MediaConvert use the value you specify here, keep the default value, Custom (SPECIFIED) for the setting Dynamic range control (DynamicRangeControl). Otherwise, MediaConvert ignores Dynamic range compression RF (DynamicRangeCompressionRf). For information about the Dolby DRC operating modes and profiles, see the Dynamic Range Control chapter of the Dolby Metadata Guide at https://developer.dolby.com/globalassets/professional/documents/dolby-metadata-guide.pdf.\"\
  ,\n  \"type\": \"string\",\n  \"enum\": [\n    \"NONE\",\n    \"FILM_STANDARD\",\n    \"FILM_LIGHT\",\n    \"MUSIC_STANDARD\",\n    \"MUSIC_LIGHT\",\n    \"SPEECH\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-atmos-dynamic-range-compression-rf-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Eac3AtmosDynamicRangeCompressionRf
---
