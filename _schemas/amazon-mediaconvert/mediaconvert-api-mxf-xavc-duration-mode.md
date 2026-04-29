---
description: To create an output that complies with the XAVC file format guidelines for interoperability, keep the default value, Drop frames for compliance (DROP_FRAMES_FOR_COMPLIANCE). To include all frames from your input in this output, keep the default setting, Allow any duration (ALLOW_ANY_DURATION). The number of frames that MediaConvert excludes when you set this to Drop frames for compliance depends on the output frame rate and duration.
layout: schema
name: MxfXavcDurationMode
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-mxf-xavc-duration-mode-schema.json
slug: mediaconvert-api-mxf-xavc-duration-mode
source_filename: mediaconvert-api-mxf-xavc-duration-mode-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mxf-xavc-duration-mode-schema.json\",\n  \"title\": \"MxfXavcDurationMode\",\n  \"description\": \"To create an output that complies with the XAVC file format guidelines for interoperability, keep the default value, Drop frames for compliance (DROP_FRAMES_FOR_COMPLIANCE). To include all frames from your input in this output, keep the default setting, Allow any duration (ALLOW_ANY_DURATION). The number of frames that MediaConvert excludes when you set this to Drop frames for compliance depends on the output frame rate and duration.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ALLOW_ANY_DURATION\",\n    \"DROP_FRAMES_FOR_COMPLIANCE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-mxf-xavc-duration-mode-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: MxfXavcDurationMode
---
