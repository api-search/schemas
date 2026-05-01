---
description: Specify the XAVC profile for this output. For more information, see the Sony documentation at https://www.xavc-info.org/. Note that MediaConvert doesn't support the interlaced video XAVC operating points for XAVC_HD_INTRA_CBG. To create an interlaced XAVC output, choose the profile XAVC_HD.
layout: schema
name: XavcProfile
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-xavc-profile-schema.json
slug: mediaconvert-api-xavc-profile
source_filename: mediaconvert-api-xavc-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc-profile-schema.json\",\n  \"title\": \"XavcProfile\",\n  \"description\": \"Specify the XAVC profile for this output. For more information, see the Sony documentation at https://www.xavc-info.org/. Note that MediaConvert doesn't support the interlaced video XAVC operating points for XAVC_HD_INTRA_CBG. To create an interlaced XAVC output, choose the profile XAVC_HD.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"XAVC_HD_INTRA_CBG\",\n    \"XAVC_4K_INTRA_CBG\",\n    \"XAVC_4K_INTRA_VBR\",\n    \"XAVC_HD\",\n    \"XAVC_4K\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-xavc-profile-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: XavcProfile
---
