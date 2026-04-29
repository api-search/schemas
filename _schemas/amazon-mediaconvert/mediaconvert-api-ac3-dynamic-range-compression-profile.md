---
description: When you want to add Dolby dynamic range compression (DRC) signaling to your output stream, we recommend that you use the mode-specific settings instead of Dynamic range compression profile (DynamicRangeCompressionProfile). The mode-specific settings are Dynamic range compression profile, line mode (dynamicRangeCompressionLine) and Dynamic range compression profile, RF mode (dynamicRangeCompressionRf). Note that when you specify values for all three settings, MediaConvert ignores the value of this setting in favor of the mode-specific settings. If you do use this setting instead of the mode-specific settings, choose None (NONE) to leave out DRC signaling. Keep the default Film standard (FILM_STANDARD) to set the profile to Dolby's film standard profile for all operating modes.
layout: schema
name: Ac3DynamicRangeCompressionProfile
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-ac3-dynamic-range-compression-profile-schema.json
slug: mediaconvert-api-ac3-dynamic-range-compression-profile
source_filename: mediaconvert-api-ac3-dynamic-range-compression-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ac3-dynamic-range-compression-profile-schema.json\",\n  \"title\": \"Ac3DynamicRangeCompressionProfile\",\n  \"description\": \"When you want to add Dolby dynamic range compression (DRC) signaling to your output stream, we recommend that you use the mode-specific settings instead of Dynamic range compression profile (DynamicRangeCompressionProfile). The mode-specific settings are Dynamic range compression profile, line mode (dynamicRangeCompressionLine) and Dynamic range compression profile, RF mode (dynamicRangeCompressionRf). Note that when you specify values for all three settings, MediaConvert ignores the value of this setting in favor of the mode-specific settings. If you do use this setting instead of the mode-specific settings, choose None (NONE) to leave out DRC signaling.\
  \ Keep the default Film standard (FILM_STANDARD) to set the profile to Dolby's film standard profile for all operating modes.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"FILM_STANDARD\",\n    \"NONE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ac3-dynamic-range-compression-profile-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Ac3DynamicRangeCompressionProfile
---
