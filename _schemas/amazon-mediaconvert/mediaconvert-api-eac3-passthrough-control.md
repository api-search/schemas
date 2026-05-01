---
description: When set to WHEN_POSSIBLE, input DD+ audio will be passed through if it is present on the input. this detection is dynamic over the life of the transcode. Inputs that alternate between DD+ and non-DD+ content will have a consistent DD+ output as the system alternates between passthrough and encoding.
layout: schema
name: Eac3PassthroughControl
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-eac3-passthrough-control-schema.json
slug: mediaconvert-api-eac3-passthrough-control
source_filename: mediaconvert-api-eac3-passthrough-control-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-passthrough-control-schema.json\",\n  \"title\": \"Eac3PassthroughControl\",\n  \"description\": \"When set to WHEN_POSSIBLE, input DD+ audio will be passed through if it is present on the input. this detection is dynamic over the life of the transcode. Inputs that alternate between DD+ and non-DD+ content will have a consistent DD+ output as the system alternates between passthrough and encoding.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"WHEN_POSSIBLE\",\n    \"NO_PASSTHROUGH\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-eac3-passthrough-control-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Eac3PassthroughControl
---
