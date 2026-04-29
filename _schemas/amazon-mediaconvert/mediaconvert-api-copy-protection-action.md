---
description: The action to take on copy and redistribution control XDS packets. If you select PASSTHROUGH, packets will not be changed. If you select STRIP, any packets will be removed in output captions.
layout: schema
name: CopyProtectionAction
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-copy-protection-action-schema.json
slug: mediaconvert-api-copy-protection-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-copy-protection-action-schema.json\",\n  \"title\": \"CopyProtectionAction\",\n  \"description\": \"The action to take on copy and redistribution control XDS packets. If you select PASSTHROUGH, packets will not be changed. If you select STRIP, any packets will be removed in output captions.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PASSTHROUGH\",\n    \"STRIP\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-copy-protection-action-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CopyProtectionAction
---
