---
description: By default, the service terminates any unterminated captions at the end of each input. If you want the caption to continue onto your next input, disable this setting.
layout: schema
name: AncillaryTerminateCaptions
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-ancillary-terminate-captions-schema.json
slug: mediaconvert-api-ancillary-terminate-captions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ancillary-terminate-captions-schema.json\",\n  \"title\": \"AncillaryTerminateCaptions\",\n  \"description\": \"By default, the service terminates any unterminated captions at the end of each input. If you want the caption to continue onto your next input, disable this setting.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"END_OF_INPUT\",\n    \"DISABLED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-ancillary-terminate-captions-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AncillaryTerminateCaptions
---
