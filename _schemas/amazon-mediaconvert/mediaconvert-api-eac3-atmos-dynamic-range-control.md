---
description: 'Specify whether MediaConvert should use any dynamic range control metadata from your input file. Keep the default value, Custom (SPECIFIED), to provide dynamic range control values in your job settings. Choose Follow source (INITIALIZE_FROM_SOURCE) to use the metadata from your input. Related settings--Use these settings to specify your dynamic range control values: Dynamic range compression line (DynamicRangeCompressionLine) and Dynamic range compression RF (DynamicRangeCompressionRf). When you keep the value Custom (SPECIFIED) for Dynamic range control (DynamicRangeControl) and you don''t specify values for the related settings, MediaConvert uses default values for those settings.'
layout: schema
name: Eac3AtmosDynamicRangeControl
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-eac3-atmos-dynamic-range-control-schema.json
slug: mediaconvert-api-eac3-atmos-dynamic-range-control
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-atmos-dynamic-range-control-schema.json\",\n  \"title\": \"Eac3AtmosDynamicRangeControl\",\n  \"description\": \"Specify whether MediaConvert should use any dynamic range control metadata from your input file. Keep the default value, Custom (SPECIFIED), to provide dynamic range control values in your job settings. Choose Follow source (INITIALIZE_FROM_SOURCE) to use the metadata from your input. Related settings--Use these settings to specify your dynamic range control values: Dynamic range compression line (DynamicRangeCompressionLine) and Dynamic range compression RF (DynamicRangeCompressionRf). When you keep the value Custom (SPECIFIED) for Dynamic range control (DynamicRangeControl) and you don't specify values for the related settings, MediaConvert uses default values for\
  \ those settings.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SPECIFIED\",\n    \"INITIALIZE_FROM_SOURCE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-atmos-dynamic-range-control-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Eac3AtmosDynamicRangeControl
---
