---
description: If you specify a StopTimecode in an input (in order to clip the file), you can specify if you want the clip to exclude (the default) or include the frame specified by the timecode.
layout: schema
name: LastFrameClippingBehavior
properties_list: []
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-last-frame-clipping-behavior-schema.json
slug: medialive-api-last-frame-clipping-behavior
source_filename: medialive-api-last-frame-clipping-behavior-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-last-frame-clipping-behavior-schema.json\",\n  \"title\": \"LastFrameClippingBehavior\",\n  \"description\": \"If you specify a StopTimecode in an input (in order to clip the file), you can specify if you want the clip to exclude (the default) or include the frame specified by the timecode.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"EXCLUDE_LAST_FRAME\",\n    \"INCLUDE_LAST_FRAME\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-last-frame-clipping-behavior-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: LastFrameClippingBehavior
---
