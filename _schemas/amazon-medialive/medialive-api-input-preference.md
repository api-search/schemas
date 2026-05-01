---
description: Input preference when deciding which input to make active when a previously failed input has recovered. If \"EQUAL_INPUT_PREFERENCE\", then the active input will stay active as long as it is healthy. If \"PRIMARY_INPUT_PREFERRED\", then always switch back to the primary input when it is healthy.
layout: schema
name: InputPreference
properties_list: []
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-input-preference-schema.json
slug: medialive-api-input-preference
source_filename: medialive-api-input-preference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-preference-schema.json\",\n  \"title\": \"InputPreference\",\n  \"description\": \"Input preference when deciding which input to make active when a previously failed input has recovered.\\nIf \\\\\\\"EQUAL_INPUT_PREFERENCE\\\\\\\", then the active input will stay active as long as it is healthy.\\nIf \\\\\\\"PRIMARY_INPUT_PREFERRED\\\\\\\", then always switch back to the primary input when it is healthy.\\n\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"EQUAL_INPUT_PREFERENCE\",\n    \"PRIMARY_INPUT_PREFERRED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-input-preference-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: InputPreference
---
